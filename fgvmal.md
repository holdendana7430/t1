代发 wailian999

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yzsmwgqc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2rehpxnfc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2dtrlrzzu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2niixdmkh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bkbvpuff.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bvoagnri.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2swxuwxyj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2illpixau.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2tigyagoq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2kyqzkcxg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2vpzfakpz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2gfnjmknj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2yuevjetw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2uhjulocm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bkdqfhew.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2wasgfdff.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2tnadkade.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2udoqluzr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kzxhhddo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oyajvicw.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2skqlhwts.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zkvmeuld.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zhhsjrtr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gzrgmasb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2euamgwcr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ndhwcmav.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ggegopfu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ipljatfr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2imnzcbcm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2anvsifzz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2byirvmcf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2eaeldfiu.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2zwnxittt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2grfozhwv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rwvjcahu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2skyhadrn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2pachwagw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2chpeindx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2auxzhqbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2juymtjhr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2epforxpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekywfhox.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2asrnikel.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2fjabegcs.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2qposuoum.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2mpbcgitj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2nmasxbmw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xekhgjtq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2elncxafp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2eecucfmg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2oantpkpk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2rfeywbvc.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ylbejoyf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2egndnhxs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkicajcu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xekkdpyy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ekjkuqyj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2qtyslycx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2qssbfndq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ilhekvxc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ekicncvs.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2vfnpwhic.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2svpwomyz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2eembutlr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2oqxsmxsg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2zncumxlo.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2cnklrlmw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ibcazycx.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jttwfquw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2sxpywlia.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fuipxlpw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nsldfosp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kjbddvoi.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2jgoepygj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ntbmoels.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vejbcsgv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2yszwuxqa.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2yajmstls.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qdltkxxh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2qksqunvj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sgtzsosj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2agzrukpo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2csazfxrx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zvtgqsnl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2axtfzivw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2brsogwse.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2uqbrbikm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hxvvsefj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2qdlnbdfs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2cstzkavh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2balaipuf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cfmgmcba.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2dppdvfcn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2coguypju.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2yweebtzr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2kkzzuyxw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2jhdnizpw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2eqtwxfkx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2pevboccs.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2nsjsnwns.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2roxurqnw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2bfpkiwip.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2avayrsoq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ekyttvhr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2wfatoyxl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jrheremf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2itvwqtsl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2wbsiswzy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvxfuzqg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2gaquyzij.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2oaqhxnnx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ruhrluia.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2fzmvzbyk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2xcxgcwvn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dilvkpxy.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2udyfgmxj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2pojdoayi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rrlnmjta.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2fpmixlyx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2xqnniail.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2anpdxnxy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2kalkhgbw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2mrrlootl.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2vblipnge.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ejdiayia.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2cgoieujs.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ayhevpau.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ugklsrsg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2awyyddah.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2olqahjol.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2omgnmywl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2gxctzbdu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2bcjjvocn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2lknyzubg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2gyasbvuu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2lrntvqtb.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2qlcopfdb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2mjghmqyc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ohjipsrz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2tuzuznjx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bwpdnady.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dwuebdwp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2eipjkfqr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2skgemyeb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2cdlrccyt.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2geogxueq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vzfggfnw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2fjuukjof.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2cdjzxdag.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2qungypjm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2blqfybfu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2audhskem.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2zbmxdrmo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jyqivwfv.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ykzestpf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2aoojmvfv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2znlpqmuj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vwsubinr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ywyipmhf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2qxndguow.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2oerultsw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ntmzgbij.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2snbgndri.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2rdznnfmg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2vithtbsc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xjrlxdel.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2oiszbnty.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2zthqmgen.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ejnztonj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2dyzyajgw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2betqapaj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2bfdggxmh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2pdddhudu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2phiplqbr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2rvljzrrh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2pndourjf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2caxvisbh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2mbqnkvvb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2tjxyamue.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2txuvujav.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2giekzfjn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2mbolaugt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kaezgjge.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ybtdgokt.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2pklekfrs.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2pcklfxey.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2nvjawkbu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ahiyiivt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2tjqnqjbl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2tvjxdpsv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2alublhta.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2umldrisp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2phcxzpjw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2gmwtzgna.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2umfgvapc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2whpuyele.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jharonsm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2igmaoxxz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2loyaqtxg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2lkuylxdb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2popjoyxe.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2wamdhtef.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2dudnbzdf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2oruhlapq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2pavqandw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2czyudrcg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xsmkicfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpcdcnnb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gtkuczfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zliojgll.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yadxmrzb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2zftdgzae.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2wetjsutt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zpisqgii.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2fkxhpwzo.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2gtqdehhi.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ywoxcauv.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2usemmaic.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2lqbdtmda.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ahsghmww.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vroksquu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tbdnudmm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xpefcrbu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2cqyxlmoo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2mdlmgolo.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2garjawai.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2qpwaubcx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ywpokstv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2eiijhrez.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ewldesdp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2stzszglt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qxjekvnh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2juklcyoy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2epfdszmu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hbituasw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2xkcinpww.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vvyujbwk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2aymriaxi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2jgmjhyyl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kxrhwotn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2zofptcft.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2daydkxxn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2enhnithl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xifealir.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vgpiecwy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kegsdevm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2vqtgxbng.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xtmaoihg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2snbtqnad.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2iutiefzu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jouyiyjc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2trdgimik.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sckthlqz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ylojjxol.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2uanhozzo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2acazzvxr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2bsosxven.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fkmxvjuj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2qrdaztjk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2gygelmnr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2dpumimsl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jkxvenzi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2sgbdjqfb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2kxzwzscn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2aouczwpz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2mnvzlnxg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vjhxebkk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ulojozdg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qalqtnsn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2gdffpqvx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2jyvvilvf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2wqtfmywa.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ovecsmtr.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2apjwgsxf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2tsxjfniq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pxwolket.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ifzuolbx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mznmtvhb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tsltodqr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2cbqbwems.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2flkrqeio.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uabtpbwn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2rdauvuym.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mbakrfbs.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2sjxtralk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eskcigfq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2lcygexgp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eihbwfac.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2laffrouq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2btwpyldf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2lpmozmwn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vuqmwkam.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ptpafneo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2kewlbiyr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2geplwfwv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2nyskumaf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2hdbusrhp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2rlbzeyol.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2kjuctfhm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2dwktjkjx.html


<!-- 参考信息 -->