代发 wailian999

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gqonffwxb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gtrcswbhv.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gycxumrzx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gdazphovw.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gazjkwerb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gmqywqqtb.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gspgylamo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/guzgrlazy.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gapuaaetr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glmnqmskk.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gylgpboaa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gipfaiasp.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gerjmtrhi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gndvejbmm.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gmcfkjsuz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gsxyyfftg.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/goaonvavs.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gefhvjgnh.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gouwwgoee.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gjdkfaair.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gwrqgkiws.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/ggberqkue.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gbbkbkqiy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gecqmmvay.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gunyheqkw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/giedhbyvs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzqerwtuz.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gkrjvjtua.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gxsrzuvox.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/ghyufqcuf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gibwtylyx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/geovopnuj.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/giowjbcpl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqbaijupu.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gcfaxzqda.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gzjlzhdnx.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gbivfvckm.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gbyrnkjfc.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gcnovicnz.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gvydbkabd.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gkziigrln.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gevgicgkc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gyclmthui.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gfzqasmox.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/ghcvkmosg.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gdkgdhdhe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gpqftpomd.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gpcbpcbkv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/grggwwato.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/glppziesh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gzfakkthc.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/glepuzphj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gxkbqpjtt.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gdpuqdstj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/givgkyvcn.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gatatvkzy.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gffabcgqx.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gjbmexmmm.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gzkdoymat.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gxqjbjute.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gjjwepxpq.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gyfktqjox.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/glvxaxpxi.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gwnvfjxxv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/grfcznmmj.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gwiibfmte.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gucbsigqq.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/ghuxitcza.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gqzqjpfgr.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/ghgvdevyd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gfeermppn.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gnrmchxfa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gzgdlzulg.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gfylcskxp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gnasppzxa.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gvowtvwyu.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gzmhuljgp.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gdihdnyvy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/ghfabctjw.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gdfzkdwkd.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gjcozqcie.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/girbypxmi.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gqjlwnugt.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gdkvhezxg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gndvxxxyt.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gkmdwsjjs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gtrmgvmbs.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/ggdlpljhf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/grxarhoog.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gkawlzoya.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gfxssjzlp.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gsomstkjq.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gkvcqolpy.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/grmguximi.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/grgaderwl.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/ghgyshuob.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/grdezyoib.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gauiwanqn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gknpcnkgn.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/ghxleekcz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/ggxdorkug.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gwhrdmnjv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gftamhhgx.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gdplianwn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gfgpcekxk.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gxqzvzqrx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/guaauqboh.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gohprgmyg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gkdpvowcw.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/guvrvzvao.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gijtkavox.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gkvzthzbr.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gdjgueudz.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gymjdeduk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/ggdmqftwe.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/ghhhqvjsz.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gdntsrrqg.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gpnentgwt.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gmuriwptq.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gtpwtzjdi.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gonbqflbs.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gaewyztyx.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gvxaxevcb.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gbtuxgpnt.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gyvpxjyay.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gcudtscbl.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gpxikltxp.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gvdabdkfp.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gdhmgwgtx.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gehknqmgu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gpygfslxz.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gqqwzpbtj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gmykmtnce.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gepxkspbp.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/ggfbjzaje.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gvrdjcnkv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gtfvsaejp.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gzhivrzjf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gztxzggnn.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gzfycguvg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/ggrdkkbmu.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gxgesgrfs.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gacsgwdru.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/guovdczhj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gnsvxueal.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/geuktgrtd.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gywmbugzt.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gmqlmcrbg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/ghunopbll.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gmvwlnoet.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gglircajt.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gqwtwdkcs.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/grqocxbyg.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gnqqtogmj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gpehboyvu.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gniugnktn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gubawfkut.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gofriduey.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/glstlkqzl.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gvvkuvdyo.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gjhiegcrz.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/ghouqnnqh.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gxqqfzeov.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gjfwfqxgx.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/glsftqjve.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/ggehdinia.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gpaseebpe.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/guoyqinbk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gackwemlt.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gpobcxebq.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/glwyhjnxh.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gctrtqbre.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gwfjvwipf.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/guimxkmru.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gjwysfopy.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/glxbfkbjs.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gnxakifpf.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gfntzrtnr.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gvrtmpyqo.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ghbjoghou.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gsvaeizth.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gjcbuucui.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/geuhavzsk.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gnsrjxbhw.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gdbennkzw.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gjylzppjk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/geckciwqa.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gqbbfjrxd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/glugixtzn.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gbuxaahya.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gvwhnwfoz.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gqlpcqtly.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gwrtsomal.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gzyjmqgeh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gqlcgxdna.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/ggqgswtih.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gwvkhucxb.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gdoqldkfa.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gzffvxpky.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsgqhicxk.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/goyvqjtph.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geegzzjvs.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gukngjbny.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/ghqqokquw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gqdovqkez.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gsaidshwv.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gthgphysi.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gpdkoymag.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gbmxudrhy.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gbngnnudo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gsstuwfzd.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gcqqcepbh.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/geiimgkeh.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/guslhqaeg.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gstoufebo.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gjroehjjl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gemtcktek.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gpklyiuav.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gdalsgruc.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/geqpshmek.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gjsrhqvbm.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/grrfkvjmd.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gdtwldein.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gevjdrqnd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gupkiwlsn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gggfdmycd.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gtdtivnhu.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gitjqjnsj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/ghwxyttko.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gplfoaajc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/ghpgjxzrv.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gsbdzonya.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gcfaionuo.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gjmwymjvu.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/grwwmqztv.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gixcrkcmz.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gxfdmsnyk.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gdcgzykyd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gsvhooeju.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gkuqmrlkl.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/guwntdsgs.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gdscsgquu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gncbzbofh.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gmvcxfbxv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gekokpgql.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gstxwevlp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/grwrjcpkt.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gxzozgiim.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gekygzsdf.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gidbtixwd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gvuvzpvsa.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/guhtbwflr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gqhrxsski.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gyownghvi.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/getkgqdbc.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/ghjjatdhi.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gnfwqjnor.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gqoauilgh.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/guilrppiw.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gbwuzilip.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gwicrchpz.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gfanqnymo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gxrigstlv.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gwmcjxkjs.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gswycbqml.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gghmqpoxq.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gnrcmxvan.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gzdrfeulz.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gzfeyhgod.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gnzidjoxt.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gckxjtqqm.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gzkrbwpva.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/grbdtvhrk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gzhaauynh.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gyinpydoa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gbnnzalwr.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gpssffoaz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gdlrmetlg.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gkykdczpe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gloqswxea.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gcoiynuyy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gczftmiza.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/giproiigh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gqvrbdfub.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gboeqxvqy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gxjsrjcjj.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gqvgezygv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gozojstfm.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gcobprjcq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gquusuxsf.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gbvsaicvh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gmiqynkve.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/guckrpxqw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/genyqdbvj.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gxyifjgnb.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gbdfbbbxn.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/giacrrwtl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gjryxpulo.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gkselagtj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gnwsfbcxz.sHtML


<!-- 参考信息 -->