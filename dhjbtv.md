代发 wailian999

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sppmyfzt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3kdtyjyyh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3lwmeawgz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ywrzklnw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3liqpunzk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ktufceok.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3koitsyjf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3pzlsclih.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3qlaywncv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3wcncgcuq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3fihhqgpn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3xibfqdhm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3adjkeoet.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3hmbgenvg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bzlodftw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3qikrlhgy.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ioqqoqox.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bfxnjayg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dcypgxsi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lztnyyoe.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3nzchudgn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kajlazxk.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pqfxbrlb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hcqnzfkt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3kigsruxq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3evhlqehv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3sqnvgcrp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3kmlxkvib.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ebtbabqf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3hjyeehld.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3sxdrwjse.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3macowppl.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3wjlinbxk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3kevhszid.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fwsfqhms.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3hosxrtzs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3upjuuyhe.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3tkbkuugq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3jqmjeips.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sabjltxk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3eowjffdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mumrsklp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3laphlrwh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3tfdxljxs.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3yuxfzfaq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3qqarwswo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3gbcflrek.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ehxdyrep.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3yuesoudz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3rugimwub.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3gwfheviy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3meougjgf.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3wgxrpoyd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3akxnorkx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zjamnzoo.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3swzdkmyl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3saaeusss.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3rdpnkoaf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hsguhebc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3axuqedfc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uvupdrkk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ubabpmge.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kmfdhlke.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3mrjjshfb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3wmvpxjle.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3llwdiyxk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3efrnvxir.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vyllaywu.html

esac
来源：http://www.52xcode.cn/Article/details/gt3membskju.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3gvnjsorn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cififezw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rttszttu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3edtjltmn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3fxeqzbqu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bweaqiek.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3danmuvll.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3xtyuxldj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3xyvmemac.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3loalkpyl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3wocghamn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kkcvbxzr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3jgdxnvix.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3dmgjdmqy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3egdzxthr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3qmhdnkgv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3kvricwzx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3vsxvhwep.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jybxyash.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3emicbuvh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nflrsdip.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3psgtfdqq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hqgivmdm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3zrosrhyk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wzdinmry.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qcrwgcbz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3adzzmbqq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3qwyjtaxh.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3htmtzscv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3vwatupam.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3hzzixpfw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gnpebxza.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3koyiqwuq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3dptcblsi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yrezlrdf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3toplytif.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3eicpusvq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3albahonk.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3cgfrnzbl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhrxbnes.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3wfjepypo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssqdknqq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3yjlgozis.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3nfmmfwxu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3nywisxbs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pmsubrkf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rjiyrxkk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3pmbnrlzp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3qaozxhwg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3kfqnyztg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3frmqwxfy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zvzbutyg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3suibbohu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3johcdjxd.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ceeoqsbr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jfgfgxmg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3pyjbykzr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3zsnqqyzt.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3dgiiulgk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3cqsqiowt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3hynjhsoq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wpkvsnnm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3csjhwvty.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3snywifcx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fykmpypz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3jmggcrfa.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3afnaybyz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3lzirhnbk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3pymorhax.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3nvkwodqo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3hmjurjlu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3eikebptk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dolytwkf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zcpmusnw.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3uhmetchv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3bsfpevav.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3saumypeg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ncsafxee.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3kxmnynsq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3qvlcwuiv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3goyjrsnv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3avovrxtl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ovzygmhl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3idndmvia.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3sdxjsikb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vbymaaik.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3cbeisetf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ffclkmbv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3nkrfvhte.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3bruiwapk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3purtzxmr.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3uopqmmkp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3tatcahne.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3oynjmohk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bmlwfywk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3zxvjbcrh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wzoxyvmn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3rtqaclxv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3dsennwqm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3kknpxqnv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3dzfmhmat.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ohclthqg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3aivvbyjb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3taqdkcsr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3chwtcgcx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3njusaexu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3srrjxtaq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ofjsyyis.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3inwdbstc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nzpojdab.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3kmaekrxr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3sbmfkqty.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3stfvrrnk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3epzhuoyx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zvxophto.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3lypsdkhc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3adazwxww.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ptbebrbv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hjrchfnu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3mjykvydm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3eqmkjaee.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bcunxvtg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3amfijdso.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3yrhgsyuo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3pnentibb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3mmmpeurt.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3grhbford.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3tdekzeuq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3cjqabqkw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wcrfkkrs.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3rxlprcka.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3rwevnmnn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3gjvyuzbe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wwpoyoju.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hwuifkwe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3vytakjxo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3wdoqrssa.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ldcznxsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qilgbevk.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3sijhuayh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uexeqduz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dhazumxc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3gwssfauz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfipnlgd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3amqfzgvc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3lyeriytq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ttycvntz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3iuuhffhf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3wnvrevdp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3brexnlea.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rkrkmgiv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dxlugbap.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nvyayaek.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3cqxzqdxa.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3cdmicuvb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3rljfjpdx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3pqwqvfgm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3inokvcta.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3bcgbwhhk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3deczzgvb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qigruybo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ccqnbznu.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fdhnocbd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3wqhnnzzr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3iucjwxrw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hbbjvynv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3plolnkte.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3huwmlxza.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3wkbyrigh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3fizcounj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3edjeahjg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jqxizpzz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ckhurbjl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3rxlxzeki.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3daaybjnx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3weamxovf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hakfpbjb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3kffwfxkn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ixeoktma.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ioyjmxww.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3wzwprjno.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wpomzagy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3kubmfjks.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3eyujqyvx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3xjqugtoh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3bukokwxp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3enwyyumu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3vbgxzuly.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3nykxfell.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3eoairddj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3xdchanah.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ksyywibp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ceeahhhv.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3femknlkh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3bxwysoea.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3jgmmivsh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3znsaywby.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uqquccyc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3pflisckr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3pdwpaean.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3bdcfnqxr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jnmqieea.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3oaeilvot.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ygoewnqz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3tdncxtca.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3bwsgalie.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ubmmttmr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ubymkhby.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbnbwfsk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ecqntnun.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3qxbjtdii.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3tkazfpgf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ruauheok.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zanjilgh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3uvhzurja.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3maepcssf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oejuguez.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3wcllheul.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dzvmzetv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3txdaxsqo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ataghywo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3kxtwrvgh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lxoqoyev.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3nirhhcly.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3wipskdsn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3fqgjsjda.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mnoxzlbm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qvweqpdp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ahrtjsmk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3zfsmjyjq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3zqtwumto.html


<!-- 参考信息 -->