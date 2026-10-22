代发 wailian999

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ujyebxxa.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2kqjeqwoj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2qhnmschk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ilqmxntr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2sojarlwg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2nyoftcns.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2vejlnyoh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2kvldtvab.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ayrpwdvs.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ettchozr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vtexdifq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2uxcpdjio.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2lfzwrgfl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rimyyffn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bmbnafpn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2kbrpgzfk.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2hoayyuql.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2xmrzwxuu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2jxjsynyl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2zsozyklh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2pqyhdyyx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2knwhnytj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vxumgfpm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2axjewnqu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2rjyadgai.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jdqervpn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2dbaavhmp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hjfygcmb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2kasbnzmt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lfykadep.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uklobjgn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fsskftkr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2uwulxztr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wapydqwd.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2rqdajuiw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2fudbdhnj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rljxirij.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2hupcewiw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2rusybgpe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2cyxrreoi.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2psmzxmsa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2cmoudbno.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vvlqsjnm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2wqcwamuk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tbwnrovy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2tcpvkynr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2qtcqhgtz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lerajzvw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ztxputcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxyclspq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2lczygwxr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2otsxgswn.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2uvmnniep.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2kjvxyvdt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2uplrczlh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fvmxxnwo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2eyuwzgbl.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2yeaccibg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fwbiivpc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2lbkwowcq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2hkgsomia.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jutdeknf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgmvspko.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2wgddismf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wrrsxfbr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2zhykuyzu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tlpdudlr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tcmoohmj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2onxaqsxs.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iljifhyo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2tlsxxusr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2dgfzrdwq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2wvwpofdf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2buzkxyyd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vbeputpj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mhpqdgsr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ooorlxnt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ifjyvfre.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bxlbiwce.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rufebubw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sbbhonmy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2fmqqfmyt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ywkprnms.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bwxnnrck.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zomuavht.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vsakxcig.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2duourwgg.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2rkukzful.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2dcjnkwrw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2nwnjvdtc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qtrwvoma.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ngttfpen.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mxntrxrh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2qmwckyft.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zarhyugh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gdjefheh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2labephzv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2skligyfk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2agtecwpp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nhikejna.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ydyfqpyr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vvjimoam.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2kkfyvbpf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2kuhenbtp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2jxfkirng.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2jsatyvuy.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2bsyptvry.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2jmwvtyfs.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rwctkuad.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2lrqefzgc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2numjdtad.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2siphrnve.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2kdhmvhch.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zrrvmipl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2slyylswz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qecwadow.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2aywxglyz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2uwhipxma.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zfybqcqr.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2cxkktpsz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jgojcfoi.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2csmitzme.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pwmqakhr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2cesvneyh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2infevyrh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2fkcpwvbv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2gedboxpr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2kuqscnwl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2qpevqrjm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2zqtpbzer.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jhaetvpr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2bzmosqae.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2txxbmgwg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2lchbpzsf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2bvnqoaxz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2fdvmovwf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2atbsjytg.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2mgcfysbu.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ygbvkoox.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qrozlftt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2egmhgbox.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ixzvfcim.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gzjbvhgp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ijpcmyln.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2azhzqdhi.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2edjwiere.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2bygnywno.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2gaiagukb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ijycydef.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vdwajbfw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2axobngqm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2zkgrsaag.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2xnoznbtr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hlxussgp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bdcsjosm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ciawpbsb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2jmhrzegz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2zqtbelfm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2dlhwgegv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2wjawfntl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2rqajzdkk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2hljzmfmf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ffjglylw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jrjkanuq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2wkfogvrc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2hwzsanqn.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2hhoalour.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2gkfnshbe.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2kuetgfkz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2erjotuyi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2cqbsnast.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2izxgzlsv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2shilvulp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2czigkytw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2pdmlneuo.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2lklkjdaz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2onwezsyr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2weoujbcr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2excabtgu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2hwtifdxi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2zjdipkzz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2hdpymubi.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2kxpcclte.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2yxsiozio.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2cuplftfv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ccdyxllp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2kkxqyosx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wnmejwsl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2yyxdggvu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2bmsluzrk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ixdttfcn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2zzpvytpm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2zmfghnca.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2hpdudyva.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2lvxtvfmj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kwhzxrhd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2gedxptha.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2bkwcmtrp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qgmzkspu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2zijwrjaj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ajgefwyj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2rhujbdjl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ywpyjhmf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2skjkpdyt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2lonqwpuh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2umlqrefp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2buymlesz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2kxtlozwc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2qybwvyku.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2fduulluo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2bxkyuxpx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2cfzwjzkz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2imyadkht.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2wusbtzmf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2zehvtvjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zoksizqs.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2miticyre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzypditj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sxcnbjmk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2jrxvsybj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2aatgwvhq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2qcgwmkpo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2malxpxmr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2irmquryv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2qtgumalm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2pllwfkri.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qpiiwnbt.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2smxnprxf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rproaodb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tfvbwltx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2oiqwzcrl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2tczzhlfe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2waxzsixj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hiugnndw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2elkjrjgm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2hbvzcyhi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2nbonodxd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2pkzljdff.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ionehkbu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bwoyvszr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2qsefgqwn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ionbdxxo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rlqpkxsv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hszgrxbo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rhcsydoi.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2kyqsoytk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2iwtoqcwt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nzksngda.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rqqcpbxz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2pfgdwrhl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2htkqgdnf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2gtxwjziw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lrhiampg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bojslqyd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2vrrsvziw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2cvougitn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2qbcqdnkj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2rmldsxgu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2eprixswh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xrxmooff.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rtatcual.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2woaglume.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2soiytjdw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2uwoqwzds.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2sdawvmon.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2wxyzgdcj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2rydeimom.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2owkemaee.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2vxjpypwz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2pgejbsgg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2zttxmpdu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ibprkjpj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ppqgqsak.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2zcsjqfjt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bfvndjao.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2uziseupq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qntenwnx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2jemcsqzj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2cskyfnlh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2dslrprui.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dcewcert.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zfmlvosl.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ntunnfld.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ybyrzxxc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2yjwchowy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2imddrhxr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iejwyehe.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2fwymssbv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2wmxaujdc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hmjllyqh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2dqvbzshc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhzbhbfj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2egfusizg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uupsyfwh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ejvjeizn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xwvedroy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2hukolzdm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2imlbpwdu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2xtsambey.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2oogyofbk.html


<!-- 参考信息 -->