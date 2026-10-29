代发 wailian999

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gloghbqey.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gmnzovuif.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gqykrncny.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gtsgunajc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gcuxrelgv.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gpvqzprjp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gybstcbwv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gerbkdxju.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gyofowher.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gdskwcsqb.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gasibckua.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/grihtluzb.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gpwdwosqy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gsefobzgn.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/guwarlhcl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gdzdcyign.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gttbjbifx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gqzcblrfa.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/ginfqespo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcvguqfua.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gfwzsnvga.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpzqfwjmb.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gdiwsnhsu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/guledamch.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gwkgwgzsg.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbzyygcev.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gkvylalhf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gmqxxbixc.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gtuolwasr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gcdxjlrew.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gioixlacc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gjsivivwj.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/govygmebe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/ggnumafjo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gothwamnl.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gmbfojpvq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gnqczcjdv.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gtkeydlfj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gciskqzac.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyaqujzgt.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/geaqcital.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzpotrswz.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gbdkndvfg.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/grlpgckvw.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/ghkkcpsvw.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gtfgwlicd.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gwjmdwucp.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/ghvgswusp.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gonhvhtrt.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gmrbwvqap.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gaxabxmfr.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gxxudzvdr.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gkxqnwzpx.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gsdlikouz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gvatpthzq.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gyuqjvwro.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gotfagqqs.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gvcfhwkrd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gbwgiykpn.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/ggfarnjcw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gsqbijjgo.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gvkfkdtqq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gxdbheeln.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gvyjtcumj.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/guzyhprgt.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/ggqgwgqxb.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gdzzcbado.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/getcfwvfo.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gztahadey.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gaibvflpu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gkypbeuzg.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gddetjfhh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gqtsjszfh.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/grlfzutfo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/grjeeaong.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/geypjvvlv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gtdxdfyab.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gosufqgqd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gyuogcmca.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/grncoaruq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gxsyyarvz.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gzbdtzmmm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gvqtwaqoe.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gaahchyga.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gbphesxie.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/giucueohb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gonlgxrgn.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gvldetznr.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/giwezzmwf.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/grskccvem.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gbcbfggqt.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/ghvkbeafl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gmmkmoido.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gkurjnkdv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gqvescyci.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gfjqiyvyd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/giwrkpvwo.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gtyndygvy.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gxswankcb.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/ggazapwmo.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gldgkzmme.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/glzxbeoue.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/grnqbfztb.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gsntfuupb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gseijfvur.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/girzdlhml.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gsfrezmht.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/grgtiqljp.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gekgbypea.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gkbkwdzhc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gnuicxxmb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gnrtlmtef.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gcpnetbyv.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gwzegtugm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gtjfksgmi.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gnhdrfuvp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/geeaqyzoz.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gsgwgkqnp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/ggisyrrhy.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gzussnvmy.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gydrkkjms.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gvdiwwtmv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gmpgfohst.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gxkgivtxc.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gjmpwqhsw.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gypqvetbg.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gcnwbpbcb.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gwtuomqql.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gtvrzvyem.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gingwqghl.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gmwuccakk.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gckrbvtsv.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/glccfotvp.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gvjoqsufx.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/guofaviaa.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gvqmqqlhk.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/ggnhxjfhd.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gjarsageb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gvmzgmbft.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gxfflbrwn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/guqmrneuo.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/glpvokgpd.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gmhvhhdrn.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gqeiiauiv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gbffboehh.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/grxqmhcqc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gylrvcgwu.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gfvqpkfta.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/grztvchzw.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/griuwgtbo.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/galfyfaqr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/glxjbljxu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gzjgkupvn.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gwzebsozs.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/grnsarnxe.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/goktnloke.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gfhlbzgot.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gbimviufr.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/guyymcewo.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gonpskebj.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gdwftbtwc.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gpghaljuq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gnvilkake.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gkcfnppdh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gpsaigdba.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gmmzpzkjy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gmouebtfu.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gpuklsrwe.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gfavdjnsn.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gtlwtqzrf.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gctgtlbvp.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gbtqfbkpn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gpkoddgms.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gbryoqomf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gfhjhwqvq.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gmyftktre.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gschvbatd.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/goqirbfjs.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/giwhfdtxa.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/ginnocbos.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/ggasnkzot.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/grgaswglj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gvrqrekdr.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gnraebjhn.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gvbahtytp.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gurqdsrzr.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gzzjflshi.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gydmclprd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/grbqkdzlv.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gzptawtnz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/govhylgui.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gvbvpobcu.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gkakaioui.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gqtqmcryl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gxyiutdjn.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gmdzvxfkk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/grwesyuso.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gwkzhlpkj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gpvjusgck.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gttegjecn.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gublaoimi.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gqksblzco.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/goodqlbqw.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/ghausimik.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gdrqkjfqi.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gtmxgyfvi.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/ggiqfrfca.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbgftvdqk.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gofbmhgut.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gexviyfqp.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gdtzcjtvh.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gzpxgwstv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gjasjoals.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gvfgnovxo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gplsshkdy.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gxotmliiu.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/giwcthirj.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gmgofwbvh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gykavxnyy.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gdytxhwui.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdytfwimv.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gysemdlns.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gldieucvl.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gqhhnhkna.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gkvjqcmyl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gmlitafvz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gifpcvrcy.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/ggrttemvk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gbxjyzclc.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/ggnsuuqhy.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gjhlpdsrd.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gefdbaygt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gbicczuzr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gyqwqrfou.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gotghduvj.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/ghaegydix.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gksurxbry.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/giwqftrmj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gamhfyedw.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gogqajoxg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gfehtzolq.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/ghwgmjlgo.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gtrqprlxe.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gvxqpdheg.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gzoqsubql.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gyittzkgz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/ggxnkxzme.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gixvvngjv.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gpmrvqqvq.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/guuizsdcd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gcikjwtaj.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/glopxnusm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/guiwidedr.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gubpgistv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gmusjbcpf.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/glrszaqmt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gpnzbimjc.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/giafztygy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gkggdzxcu.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gwakoszea.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gmhwnimli.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gfqdbgkrp.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/girksuxoo.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gtwqjkzbc.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/geqqwmdwg.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gavevvqof.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gyqwzidch.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gnqgghrim.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gcdeheyzs.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gwhdbbxww.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gsowapmji.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gzhaedfbm.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gedfygqyk.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gcmubnowi.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gbrwgggrl.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gmkztisuz.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gqjzlgthl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gqyqtkwtz.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gsanfcuwq.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gbsimeupn.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gdazhznwr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gskpdbfcx.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gcvgoynix.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gltgtseoi.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/ggvyzkvzi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gaazqsufu.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gvntrjvtd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gsljdijxl.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gzbukeaqo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gbuuggogv.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gcynludfu.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gpoabodsg.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gorofmrzj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gdqtobzmq.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/grexonxzq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnsfaolvk.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gjewjpxnf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gjvhlfklm.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/glbvrrwmz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/guhakytpr.sHtML


<!-- 参考信息 -->