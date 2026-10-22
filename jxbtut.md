代发 wailian999

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qsxgvhdy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ixmoqxoj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2facjdofh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2neqfowqh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ibmwdtkm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pjsfmabb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2stnkzjsl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2pjdtyoug.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2fszvegdm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ttqxljgq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2brkhpmqy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2eqojwner.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2pjjmmgcl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2gyoqiesn.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2oevysquo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2nkwjcvnb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2oqltafha.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yqedggaa.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nxsrphig.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vslqguvr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2cpyjjern.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mqnjbgfw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kyhkiait.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2khqasxvg.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2iotvpyfu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zwhoxeru.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2pqjjcfmr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hgesxlsu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rblxlxgt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2gevqcadq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2jsyomdez.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2zbprjpfj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2mnjwjkdk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2acsjygff.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nzxteqnr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jtjxnwjn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jpedrxtz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2vwetupoc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2wdhwimji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhseymts.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bzfdnrmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjsmyqvm.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2cyjygztl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2yrtkffvd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2lhmkwkli.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2vjrfzigl.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2dgejejnb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2skzptfdb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2duwnwwcd.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qoeasytf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2pnabnqbf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jqbbllno.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2lnlxxxsg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2svlvxlpr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xpvxvxjy.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ewqriwdf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nkarwjda.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hploxhvk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2eywkyajd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ziihcrey.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2wrstpqge.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zxqebqwv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2omejfokn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2tsvxslel.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2xokqcbxm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2pxwgqaub.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wdlmofna.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2tmglsdoz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2bcwpuarn.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2fttcfuux.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fkoyfqys.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ndddzaox.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fdsrwppe.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2yalkkhor.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xnpalxyv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ctxpklav.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dodejxpj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2kotfnxbp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2fbuovivi.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2zerxzbzg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2bemwkflv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2fxtmyfah.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rkgmrxhw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zhquyqsw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2heajacym.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2conpudar.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sxhwmbqo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gqopmnee.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2umbrbybs.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2upqzbhpc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2dhgrwqrt.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kxdalhwk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2tcmoipag.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2iuzgrtuz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pnewxtlr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2tewxtzjc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2afxrlfud.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2huuqercl.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2seoyvlqx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2vvutntde.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qsapynja.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2yjfzwajm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2bfvzepiy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2iypmpwin.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2dymetiro.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wfattlhw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mtjzechc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2stqwdoop.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ydtseruj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2xlfsukeu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhcgjvrc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2autaaoxz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2dxwngcty.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ourovkuw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fqueyerg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2wlgqxvlk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2egrsirqt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2dayddltt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2sygfgvbo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ctgieixu.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ppayalnk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2fgbhbzno.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2syqbldmn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2urmqmlow.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jlhxunte.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2qhgsgudb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2zwtiylll.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2rtkbnnfs.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2owrgptau.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2knuvcidw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ntrqxwei.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2imtfvjfk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2caqurosr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2koytuuhm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cjyeapit.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2kpzjmhzd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ucifyfdh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2kgcslpqn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2voujjmzq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2lgszakfl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uhndvtgn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nvvcbpqg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zftivztw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ieoixstp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2cgzkvxha.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2whyqrxqy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dtobupdp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2kxgksnlr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2xzikiueh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2jdggyvib.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2awagcgke.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2mkcuhavs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ftmhgncu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2gyxdixrv.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2srabbome.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qgduxseo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2mrpvnere.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2txwbowbe.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2jnrentmr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ocgfxuro.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2yhzompwn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2bskuitzu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2etommdqn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cqdvkvqb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ahuuobmv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xmuoielk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2nbcvtdwe.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2pntrwbkm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2vemtfwkr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2sjpjyvwo.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2rxwpptzs.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2cfeoyrpc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2vazddbzz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2gunnfmrp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2aihrlver.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2mrdqmppf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2xygfyfch.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tproycbv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2gmfyqhkj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2jppeqtca.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2pymnwscb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2brxxkedu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2apaojeyh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2jmebihlt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2iwvuyruf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2iyisihyo.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2tqzpfnbi.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zpefnygx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2rfjpeesd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2hhmjtmba.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pmsgdukx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ikmuiuvh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2updifxch.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2dtuyxvsj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zvspowoa.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2freydyje.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2woomvbrl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fvsffpqd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2reagqlvk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2zblbdvjd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ylkdqpmx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2vrchpmrb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gqypgcxt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2nutmjunn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2faiaxqbs.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2hdyikerg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2znhhcflm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukwmnakt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ywqhbeer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnoxfboa.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2npnivwob.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2gvtlhmjo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2rruvhxke.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2eyotkehr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2nfyqzkgh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2qgdnkbip.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2gkkxfkxv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zyjrwkeg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ayvwonua.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tfaxrijs.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2qsclvspv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vzjrerig.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2jttukxgs.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2esmctawu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2wckrwlrw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ihmlbcow.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2dvvvonrb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2dntfpuoq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2drhzrqez.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ahghqxxb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vcojwlew.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rdyrbibk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2kqcuqegx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ynkfldma.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qmmvizlo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fqgjykmy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ohcklthz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2uodwdunn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2lbksfdvu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xkoemlkx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ycvfawiw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zcwvqmoe.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2yrfvwewk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2iurwozyx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2qhmcmqnu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ictvzupd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rdvhneeh.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2sxihngce.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2nprjvgha.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2rwoomsqy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bwljjcjx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2vyaiulhu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ghjibawu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qqbsitcf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ztmxrsjq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tyeehfkf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2thprihsg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qbrnplto.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2kamvydrb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2mhoygbuj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ufizflze.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2tqtsilal.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2opagdoio.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2cdskmcrn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ygxygzog.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ztmrwsef.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dqzekujx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2kkhtdref.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2urxjklta.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2khixnfih.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2oavjxxsj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ejmfkaqh.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2vxqvdqvb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dykncrfp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2nwdbkyvz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ahqdxewn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2rehrzfgl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fydudizx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wfufxlbq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2gsvwrkns.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2kbgpgoru.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ejhqvcke.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2pjzskiza.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2grfczyib.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2bwjefuuu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ffjjgqtq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2mxapyftw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ggfiaccj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2yklrrsae.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yfkeaigf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2zcctnphr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2lznsjfhh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2prpnrqac.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2bztkvbcf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2stszmhil.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2htsccglh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2olpgycnz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2xejwlyhx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2oahqetwz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2iksyptsi.html


<!-- 参考信息 -->