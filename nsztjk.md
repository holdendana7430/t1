代发 wailian999

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3otrhhhvq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3mtozpxtc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3yscjuspm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3qtexosbu.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tjluzpoy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3gtvbrvsr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qdzxfvcx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3gktiruab.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3khgdfiws.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jlvaddvt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ovzvnexx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3xbggnqqo.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3jykeaman.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3anbffjyb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3hrokbasg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3upetcpah.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3keevhwgc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3qohhfabq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3bnqzsaor.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3fdhrbdgo.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3rpsljacp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mbkoqlfo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3glzdoakd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kfivjgcz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3axnawmof.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iidnscau.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ndfcavmd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3phwtsyya.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3eggocmsa.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yoicrtfm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ltvwtzlx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3kqdabtth.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3rsrgocar.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3bnungtwa.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3mofqhhha.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3nryfumgu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3hjccowzd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3xywqwsmq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wsvuucwo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3mmlokocl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xtltyola.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3dtwswnsy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3vesvfkfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wactiqnv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hsmogrku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3giuqochj.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3eibudepy.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ddiftmzc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3fmnbgruw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3uwrvfcvt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3cynsnhxo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3xhystiuo.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3cscznmqo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3zpizewlw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3dhfkbwij.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3bdeypwao.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3amcelwnp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jjoaoxnl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3atxtilpz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3gykhqbyv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cptxbvwn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3elvamiye.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yqrgsblp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pusbijwz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qfanxfst.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3etwptyfc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ryrrceez.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3fzekxfcg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3kcxsqfyn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zgigpuvh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3fyuqlkcr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3twxtqyel.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3pwsgbcat.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3tjlersqr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gxausxqh.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3akktulkp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3usgfeqhs.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3gvfcqjdx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uuulfzlu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wubnhpjw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mwsndfgu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3skwwkhah.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nzwuyfeb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3lcameqaw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3sckqxhlh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3rrykacfl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3wuaxlugd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3cvpjrkds.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3syrkqkbi.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ekefwgdy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3yewvvrep.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3htdzofwa.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3zcymbgxi.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ezhfqcea.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3tamjqbcb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dqvixogn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3apxryntq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rtuxggcu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3dkgaoisf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3gbhevjiy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3zlpvaxvl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3upxyaiqc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3imqgnttu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3kwviecpf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3tqpatyga.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ktftyyrn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3fbxdfmqu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vznhlefh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3dipamjbq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kvveauon.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3xkvjgegs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nidwcmkq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3uuoxyftl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3pffnjoba.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3kopulbsc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ovweojie.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3rrjstzrs.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3cxpemahr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tzioytlz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gkumbxgn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3nwhgvezg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3trbwaykg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3azcchyfu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3jokprloc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3sroyltlj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3fqtobsmq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3onbkcyav.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3dkmscrkm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3zcwtqlva.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3dtlscxii.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3gbvuxlzh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3kooazjns.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3iqnwopkq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3zcpydypd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ngylhmcu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3hwunvzhu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tvhenkqa.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3hpeybsze.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3sdjnyhfw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3oiiuikjr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3pfqmkyyc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3duduknvw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3blntliqg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3njkfvmpu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fsoawejr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bdxsbgpb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ukjsxjjl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3fjpenyen.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vpaksqbb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ylzuggpy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rkpxwvow.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3juzkfavv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3wxgqdhtr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3djlwddyc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ecnsotmd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ndispgys.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3jxmdgngw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3zdtwzsjx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3rvfziizd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3vcvzpyey.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ntqyutjb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3pezaeskl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3getoxsvr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3smozkjem.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3gdycfaph.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3jbtgdbec.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3dowcmbol.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zspwryaw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3vfzhbune.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kglxelsg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3pwfnbxpa.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3cbhajdwb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3sojwlqnn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3undlorip.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3fmajfbsz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3zdxzybyc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ykcbzwhw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3iyngahin.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3veozfcyx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3yrrzenak.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qblgmluf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3cuffofww.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ngsngrhp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hpbtbsqz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3zcytvgqr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zvhcmnhr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3buywgjpj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ijlbiuqf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3kolyijtp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3nzixtlos.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3gamiwlvy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bdddnlzg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3nrlhacis.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3izacdsqa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pbstjvhs.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3gazqcpgp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3yktmivqx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3cpwrburj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3abpplqae.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fszmksox.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3bztnxxdz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3jrkpnksj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bwysddxq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3qarairrn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ztqqspxo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3taspovll.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3zhoipiao.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3bvzxudrh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3anerwhxn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ehubvtgi.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3lnjhlddf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qqimtyri.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3pghywijw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gseunolh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ettmfvro.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3kucayyea.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3kgaockgp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jhmezjmk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3tyyadpbd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3eayhramp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3kwbgmskt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3fegamppx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gkirabvy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vdnubshj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ijcorvek.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3urmwxrsm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3uenkoyje.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3jzejfgqb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3pgcvwath.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3orxysnvs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ejtvutrp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3jsnrhguw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3icrzftwh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vwdtcexi.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3fzokwmdz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3chkpmale.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3gduzintf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mupgfzst.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bjfpbbew.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3usmkudek.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zexmcjow.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3iowzlevd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3auecumpw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3weahbsnr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3byvsmslo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ivkghlbl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3vjmdmjhx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3rvijopup.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zwkqszlp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gjgkgxap.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jxiwobrj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hivpyumv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3hymwkydx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3avhpzakq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hpggczcx.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3mpaohzft.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rroobjzr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hvyvembi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qgcgjxyo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zoiufrjl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3etqvncfb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3eymqftum.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3bdjycpvf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3kjtrmvnk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ewnhucsk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3portured.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3bwrtzuqm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3zwzdhwwv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fgythbhy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3hwualwmj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uwiwcpwn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3lvlycmrm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wzndnxmd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wkonlstf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ozureujk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3iuubblob.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3exfwrghx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ahahhdzd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dgpgjfvd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3urskfsdm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ceikukco.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibkfyfjl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3grdfofhl.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3jtuiebgs.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3kfntqkdp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lrtljuqf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qwevrtqm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3djdsniic.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bgqagdmp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3araexotl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3njndpkul.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3icjdshog.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3pfkcicgl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fjpcucpa.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3phrefrxi.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vajembvr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3cbgilgeb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vgpoufrc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3idkojrda.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3tspvsbyq.html


<!-- 参考信息 -->