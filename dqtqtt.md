代发 wailian999

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2drrjzwph.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2rjjimeus.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2wuuowigt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jkcvpkhx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2oweqocqe.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2idijsgrs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ictxborx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2mxwlozvz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2mjymryzs.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2tabzrvkb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2fcelrtjo.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2hqgeilzn.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ovxhrsyh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2zgncxkyn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2eukuojgw.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2mjdphwds.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2qrtbydyi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wnwlfdcy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2usyyrizd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2fggcrcmk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2gistoyew.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2isuqyoha.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2invjhstm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2nhmihvnr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2lnaumzsd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2vxszwyau.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qpottqbc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2oyqwfted.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2yojothfb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kjvrhtdm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2etehtwea.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xooplgmk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ttwibzol.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2syntxsau.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vdwfzcch.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yylopsrc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2acpqypgy.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rbbxmver.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2yctnfbpa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2fevaxpyv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rskkeykj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2cbnnkmqj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2bonlhqdk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2iwjptgvr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2lvyaoilw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2bdfihirm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2npusvfyg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2wttjphgv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2euwjhnoi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2dtpztwlj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2jivamsez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgxbcmrc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2mfisgsyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gnhgpvsu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2dwpzdqrb.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2dotkczlm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2gjbotvak.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2jyevlekp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2lxwpyjcw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2tjiwpbno.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zxflvnlq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2fjsphuru.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2jtdxeoud.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2mcnmcbxk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2uifxfpdt.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qkkezjbr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qduimpvs.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2wwygmjsb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ldrqqrdc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dpmsisdq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2suzodhnv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zfiblzwp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gucdkqdy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2kzmdpqtv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ganhdpvv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2vrqehsee.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2cjnwcmho.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2frizjupg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2iotnknfj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nnmjkmcs.html

esac
来源：http://www.52xcode.cn/Article/details/gt2bsclnwkt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2nfdubqww.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2crhkupjs.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tasqnxuv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tqjsemhb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qavklush.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2maitjmte.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zgyhvauo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xkptbwkq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2xjhnvumx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hnmnlpai.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2fuuvbpec.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2wacouxmi.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ziapyvxq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fycbjqti.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mztqbrex.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2cenjrcpf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2qdwsevzb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2iamxnvdj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xuzfpfyl.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2wojchkfy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2btpjrdhh.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2zepbxkac.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2iydykxcn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2stqfrugj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mznesyht.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ecfjmlvq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2kbqaixmb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2qrqtkexx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2hnbaquyi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xvhuqeqk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2pzcrabka.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2raobobru.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2mmtzmitk.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2omfznbyc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xljafcva.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fnbiivoy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2utkmwakk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2yfomqdbf.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2gdavxmfa.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwzpeqfl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2pjoiouvj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2idgwqrhx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jszoutoo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2qshbmfct.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2gxkiiutx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2knvjxodx.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2bpayrmvv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2tbhgaiso.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2tfwnkldf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2mwwicxtc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2bsshopak.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fcboitjv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ebhothoe.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2capwawph.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2wyqqasfr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2cvnobnuj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2nvbqozgm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qstzdevg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2rtyllktf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2okerjuvt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2mvnqkfxg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2xlnermso.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2bgtnlwfi.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2iclysbqv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2itepmjqu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2mughjgcw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2jqlhomgd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2qzqgehaj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2oldrsgfk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ewnceayt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2qjzzliti.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xtwetbgm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2suuacrpl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ghpilndx.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2toykhkzk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2vlsnvpay.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2wdgqlhsl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2icmfnsql.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2futomwbm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jmtfglqz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2kcfopwpl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mgcifwka.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2fhqbhdve.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rgfwgcgl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dmioejtp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2utxoptyw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2tnhxwzzg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2kbhjcrdr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2tcqhjudo.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ublljzhq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2slglizmi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zwhqcegb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2mgdlkxot.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2sbdrirnd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fmrvlhnk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2yslizkgv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2enumvkbq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2mhbhastg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2vxjvydoc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2qlvsbphi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ynvingdj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2uqrpwcpb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2bruhggif.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jumfaahu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2hwihcnrd.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2weqmmwaa.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2jvhiuyjx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2vnjghwfm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ljvneyie.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2vsudjltu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2eaoddfed.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2khfihylg.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2sbucwkiy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2urnqsjnp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2hsgirmdj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2snveezep.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ymqtrqnr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2xkllvbst.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fhdwjpou.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2gwdoeayj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ibwkujez.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rjaactdd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2vlhlbidv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2vsrwzode.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2cqluekbf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2oecgwtrr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tjttdrfp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2fyvsppwb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2erebzwyw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2znxqggoa.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2jtjycivp.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2yvrddsxc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2vuyjvcvf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2xshmxruw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qogxbwfy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2poootpcm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2lgmwaout.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2raifrbjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmaqvytr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2moikaazn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crvbrbgy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tbmoqibe.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2rmzkdwcf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2gblanrpg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zfcqdqiw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2iehoqwgb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2tjapgvda.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ckikctxe.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2eshlcjfg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2enofkmhy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jhesjolf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmyzvird.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qyuzpwus.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2prlcenjn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2chdvuvbz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2txnsuhsx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ehskgwrh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2bmuldumf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2tjyxlncy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2cbzbpict.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2gcsqpbzd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gsrvrzxb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tlrghvzj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2fynjiean.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ddakplwz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gkoxfqcw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gxhtktmx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cptkflqb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2wvoxvbef.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2peqzeuni.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2omotvwth.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2vcfwohoj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2afettteb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2wonzopxk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2oartgvbc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hbcmoxal.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cwpfntuo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ammqeucs.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2emxbqerb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2kisslbpl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ikivrovn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yalidjmj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2jpwrcpmx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tamohneo.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2kzpumlxh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2opfnykmm.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yffguzbt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2xasmihnk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ikzzdvdy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tmyiclii.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2qrvqhfqf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ohkfbgtz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2bgwsfutr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2baeageto.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2xsroexvo.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2mudmadbv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2dhmskxpi.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hrsncgjm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2jtgvijkz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fniypqvz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bmvaagzi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2imwtcrbi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2abslftsg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tembtnxt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ujszbfie.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ytuxkqms.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nnxomqtz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2nrlfnmep.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fljsunyz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iygmrtsm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2rscyxtkx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2wexzmjrz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pwzakhlk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2hfmawiuh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2yrwnalzw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2xpsmxntb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hwahddfk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2aimbmirb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tfxogwpa.html


<!-- 参考信息 -->