代发 wailian999

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2orgwtvaf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2bbpaorth.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2brozwool.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ruqqeemo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2jgovlmjp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gypkkzva.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kxemtygg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2npflkhjm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2rvzwdrgf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2wnivyhxs.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ogysraay.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2fusrmbpa.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2kmvybrkn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2awbqgyti.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rqhsaogz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2mhqrqvvy.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2msflahbg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uhgkqjsn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2upfwzdyr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xnjvxmwl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2rphawhkr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2txlbcqpr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2aldjaclz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dxkwojnp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2qwrlevgr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ejnwqjlo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2fosxuonh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2iomgdhyk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2lbfnnytr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2myizrqgu.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2jyyssyru.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2cycsxznb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2zbhxeliw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2fposzpsw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dkquawgj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lpwwrbng.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2disctpct.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2iszpvsvg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2btvcivyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2koinslee.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hovvbtdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ztdifyqn.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xmnhzbfl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2jxsgeabc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ttzmnyxd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ohjqzlvn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2vqjuixgc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2oadsuljz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2vxwzxinu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2dovwzfrf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xndiqkxw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2btrnqpvj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2dpvwosei.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ibquymfd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpktofar.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ntpclnbg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dmyggdma.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2byliclky.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2fnimxaox.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ynuubpiy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bijvgwab.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2larlpqia.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qbhxlujy.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2govftnrh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2nsspvrxn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2sbtpdxdd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2lbatuoos.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2uonouvra.html

esac
来源：http://www.52xcode.cn/Article/details/gt2lncwjhcu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2dhcrdhbg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2sazqleif.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2eyoxrtro.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ynrfaenl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2prztholp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zaroejhz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xouywjrq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2bwfdfpby.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2mtwlrksd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wiixqqrn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2vuetkthk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ihtuwqdo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2demlbysf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cmkknsam.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kgpjqayg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2pedbhhcv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2lullwkvx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2itrblwtg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vypyuvar.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2dnrwiytx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jzxznwzp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2uropnfrk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2klrskaxv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2tubhdxak.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ukyarbxh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2snhvdciy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2tqifrpmk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ouubhmsw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2tirprstr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2puxgoaxz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2wejqmjdv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2spvqfljr.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2iigaazfe.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2eykjgqrk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fwbeijkg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ketybfgn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2lmzwflbl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gqrjhnht.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gqrkthpc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovnuubyy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2xsqomqua.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ffkcwedw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2gxnrmaoj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rgzldndl.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2qijhfrrg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lzdnhdfk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2wkgshadh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2cmdstlrp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2woghhlvh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2zfxkhedv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2pkdylelq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2iczbwohj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2bwkngugw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2lhzbeaub.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2mpijgzjc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ihwcondk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2fcgcdzzr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vtihzbdm.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2oklvkanw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fzghjluu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2jmoyukrd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2gxxpabov.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2jxhzghrx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2koqonedm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2vcteqblp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2xsadkloz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2mfbvicss.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2htmmtkbl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ywwsisag.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2sluwmgaw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2oggdszaj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nphwvjsp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vzrvsorq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mrvzshgn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2wkdzapet.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2oeraecwz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2qncauuva.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hbngoyky.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2xamdfxgm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2sbiitpkp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2eivxardr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2fiysirze.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2bxvqwxlh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2dbaibpxy.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ytlrodvk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fzovvzjg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2hrmyjiau.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2roxjqsoz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2jigsoohk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2fhjvbsxp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ehcitbnv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2luyrhmze.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2bdmyyfgt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2gpqjzrwr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2htrovsgw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ckpsqhvm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rnxrucme.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2lnkbctkk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2jsyquaog.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2gevylulw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2gwyhumuz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2tivnsufe.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2owusizqi.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2bzannwga.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2xrduixwz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2bvaolska.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2hoyiqmqt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2exdzxurq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lqgzwmwq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2lmsiuflb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2bffxtltz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2bgiblltz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jdckbbyp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qeefhujr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2tasiniik.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2cbvwedks.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2vvepzotq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2aoxvdehh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cbwuohic.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2mdkwkbss.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2jfrwknpo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gljyzogx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2jdtgfoev.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ominytvz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2fuehzdqr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ltxjeida.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ruzuucqc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2leyxwnoz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2nrwcargt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dljcocii.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ukeopwkk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2figkuqnq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2wijdcobj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2bzwnnyhv.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ehlnlnew.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2syjfekaw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bfxfqirs.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gnfstebq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezjdgtdf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hpbbkypf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jsyenuis.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2duildngi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ffhlaxrj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2xbgqzuss.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ezoqeecm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2obqexpnd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ktpbvgna.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2qwrpanvk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2edlztigh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2yksvjwdo.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bfeohqdj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2upghtjba.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cklrtaqy.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dgdsvgyq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2edfhljtz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2iagqimfw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xthvvksr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ksgkkoym.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2meposogn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2acmzwlwn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2yahcwoko.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2fxyhofhq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fdlvfdva.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ldhpcjiq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2dnbmorff.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qtbxmeri.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ieuhnuqf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ffcbkoir.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2rocgabgs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xzneryid.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aalknewq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2rfnpyopm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2biulygew.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2upzhybep.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ptxrrypy.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2jcbthvuo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mxrfmudl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2xkrjkocf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ixrprsbj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2yhithwwy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2xzrxkoqm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zehifxpq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wfqufawp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hutnpcax.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2qtrjwesg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ktavjmfc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jiauwvex.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2fbthruxr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2wrkogirx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qxaktgqf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2bemlqgve.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2oyszqrwq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lzzrnujl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ngrxpsui.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2fueoldkk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qbljllod.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2vqthcmur.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sqzxvevk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2kxyjjqha.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wwwenmtk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qkzjumhu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2zlvbwncg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2kqnqznmr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gotbyahj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2cfkfdzpa.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2fdtysgii.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fvjheovq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2aqrnnpzg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2fpnzzewl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ieepjbgt.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2bwaozpsd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ulajwqjz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2kyprwnxs.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2hlgjnyun.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ofpseaxq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ymceuaft.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qrccghgi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2qndxnkkx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zvkcegdq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2fyzjcdjo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xbturluo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tgzyfahj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bicmwqmu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ivuyccsx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2qiwbsrse.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2airfohua.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ssotyjyi.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2cerlxjco.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2rhtlpjhg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2bqsbrmfo.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ijtwmbep.html


<!-- 参考信息 -->