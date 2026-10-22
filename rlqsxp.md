代发 wailian999

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xwhfgwma.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2taqerrzo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2nfbukjke.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2pepsjddr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fqhtyupm.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2pdlpirnc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2oycqtrij.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ohqdzbic.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2izisisco.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2zekhjcbx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jwwxznrs.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2thjrjnye.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qymbfsmf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2dixssavj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2uyfegizs.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2lncbqroc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2lryeelhu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nkeeoetc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mjwlmfge.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ihznepce.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2mhaztcaq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2wbwpkiqq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2dkgofmzu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2bvtifycm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2uzyogxbu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ggaxcohk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2abckewwk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2zjhprita.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2pgpdwcus.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ibqjkmpp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kaqsooou.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2thxsekpw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2mcqdnekt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tkdkcjua.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2esucrkaq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ljegtfcm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ssczqnpi.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rjudvxld.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2wzecepuk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2lofhtsyn.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2onccjbtp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2cclosard.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ogrytqct.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2pclskdso.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2gjgnvzhl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2drfaatco.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ptnmoswt.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ulosuokn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2kdxyweyx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2tbsuisci.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2denkuhkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fsexkusk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nlzfwqab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yahqpbmb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ramsajjz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2mcdyibag.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zhcoxllr.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ukrikwhv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ucsloeun.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2wtzeqqog.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2bkppomvz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2jiezxrwd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2dlnkzwya.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2fwslykms.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2vewegyuy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2bdbtccjb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2thcbvdrr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2lybqoufm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lshjzprr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xyqmsiuy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sbcxtsiq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zapboigq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2wxgwcajy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bwrtxmqk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2xxurvyya.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2iybslpdb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2uexawset.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wrqirbjp.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2msyohfnt.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wwjdibeu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2qqgwxjaf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2iertnzhn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mxwoqzgn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fzwaymhs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vggpdcww.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2mjejecht.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iatedcwz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kwpdlrhh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ririckgj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2chlqouzp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dxggfjhs.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ctbfuqze.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2koauqezs.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2yxcqgtrl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2bvubbpih.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hcowlchv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2qwyueacb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ktbtsfgf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2peuoanbm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nagyespw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2sxnmuyji.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2uxzkyhua.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2fgejnpge.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qvuiscef.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2rwamtzrk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mlduwwxn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vxgurbix.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ysguussl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2yxaljtcz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2uxbuzazq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2dvxrffrt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2basakjwb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rdvbgvfm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2uawljzob.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2mfptoirx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2striwezr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2tuadlcjd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jsludfby.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2udfzziod.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2kycoirwp.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2cakaabjn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2pykepwpl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ndcwkbrs.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2lzjmmxtf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ppvcakwj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2anwkvxot.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2yjgwovln.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2oltfkrju.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2bdanrtmu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2hclxswkt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2brhiycsu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2psfqkunb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2oldvowtl.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ainsneoa.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ptuzuoqi.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2qcgiwdfe.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zlbpgvbq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2csrunsbe.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2zunvwapx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2tlxrcirv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2onkjcchb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2accwthpb.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bwdpgsgk.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2kcinxykg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2snzkptxs.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2zybgcbwp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wnofelpj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2wnzncjzy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2chlzcrhl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2bezvceil.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2kojsepmi.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xozugjhi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2adzxbbjx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dqestljw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fxswsltp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2tibyqqyj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2jpxccafk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2pywmjrgw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2iblugzlp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2fnjbgbgb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2akgctfzw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2enzxkxwc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mnvvpewa.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2hvilowph.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2lhhmyyjb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ebnirlzq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2otnnbamb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2iadqnvhb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2pcgwcjqh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bybzwvbs.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2isvkbuzz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2lorioiij.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2rouaxnst.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2rdbxcsrl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2pufffypc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wdvnurih.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zcqzhmcm.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kbzalwij.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2bwmxgucj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2kupdwwfu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2oecgovue.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2kigyinii.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2cckuvfup.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2vubvglpj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2gyaldpph.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2uirdkbrt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kansoilf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2kinfnqie.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2tctzpzgg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xvbhrwdk.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ctkqwail.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2uuilgutt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2sdfvhoyw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2pbmlgfdz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mzefxxec.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2qyxkiyfn.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jpibxbgf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2oukqdwdw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2yhmwmzza.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dpbibblq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2szgrswnr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2jzchpxbw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nmjuytov.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2nkqzegkw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xcogstot.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2jwbalcfo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2spuixlvc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jhyykela.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2rpdhrskj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2tcdzviry.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jpxxbpbv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2qiskbzbj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2veihiwxp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2uodcvmur.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2uhhxbupu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2lcwhxtgo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2smjgwnug.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2slevtynv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xfsrryol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwlebifv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2arewshmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dadollxa.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ubvdcarb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2rrcntdge.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtnyaheh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2aicxixhg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2nnjtphcl.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2fnbleyzb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2gasilabv.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2grtdqvwi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2zhlfwymw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2oilyltio.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hkpicdyv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2klqlloqd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2iqfcilfu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2uexcahck.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2rqrdwujf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2wpxnfsiw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2jjxxdijw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ksfiynjv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2pvwkmhvo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2yvwvlhfv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qvfscvbf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nwcnqzwh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2vdzhvzqq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2krmmiqlk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tswijiks.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cprggluy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kzrjzbor.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2muwfrxjt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2uiwtbloz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2nsugjcbv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ihuqonzh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2miupvcef.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2zmiadpua.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ebiwylus.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fnwvlxgc.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vujcjjja.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ooghlhsh.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nlxuyjaq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ihrjzpos.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2mjrmykaz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wlvfzhvr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2zbykigjj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xvxcxysk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2kqgcfeiw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2nrqjlfuu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2egrlxvro.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2rotaxrlq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2tokkdogm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2passnaiy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2rkboxmqr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2kmkblhbp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2shurhfla.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2oezrrwwb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2fxgrcgoq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2slbmjjtb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gkeyktif.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vxfzkbba.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2brifqqna.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2cgtvyuev.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2yujybord.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2kwtahgyr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2hsixkgvv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2cxzaajww.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2chrrfkao.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2kqmtcltl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2azopwwtb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2hzszfbhl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eynbhntb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2svyspiug.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2tgkakmev.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2uxoemmlc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2grhgtwvo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2jogwhwsw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2bdhdumtb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2tjpvkcbv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cyryffdk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ajvvrsnf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qjsnmxaa.html


<!-- 参考信息 -->