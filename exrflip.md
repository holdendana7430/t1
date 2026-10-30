代发 wailian999

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gxlogomvb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gzdxbhajd.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gmgyjeasy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gwmwyfami.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gtsfwsukk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gsimyowsr.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gjoyqktyt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gmfuhjvkw.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gkakrhttp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gmkkevvfh.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gziixfjby.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjbhnyzio.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gcixvsfvy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gltucncoq.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/goqjtgioy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gopmgsxgt.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gwrhededk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gngdbanwt.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gallstvfo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gaiugpclu.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/goyuynkwr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gauvhnpca.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gexqdnclj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gqzwukszn.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gulwabjol.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gqhftqdrn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbryafqai.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gmbjlwrwn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gjbzyqjcf.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gzwidscxc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/glrolrdje.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvnymwtau.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gjudzciyc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gexynvcbg.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gzqrkaugw.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gycexrbjn.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gwnxhxdpw.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gcxmbajrv.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gaghivfht.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/goibuvpnf.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gufnxahbr.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gejttxqta.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gaqpbsioo.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gbpqazujr.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gcpmomxqn.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gfhwgzeqf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gcatlrbsz.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/guoasmoos.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gabrcbhxw.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gufzvsyrj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gdmpcxojq.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gfsibftct.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gxdaivkfw.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gppurgmsy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/ghhgtihpd.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/ggwqzysej.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gapnodzoe.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gldbyglfg.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gxxaarxbv.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/guexvbnsi.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gerfsdiwa.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gdqxwvxjb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gwvjseydb.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/ghlktyflh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gjoyjealu.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gcpqlvwni.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/glaghmgqe.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/ghfygjmvt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gwoerrgcj.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gfwllmkkc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gczxglwbd.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gwjuywgvt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gemyniitm.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gtmkflwvk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gawdryyjm.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gudwhbfks.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gqiqitowf.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gkrohoxbl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gmkgdzceo.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gnakwrawr.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gcokajaju.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/geetvjoen.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/ghxuahkav.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmayesjax.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/giznsyfxv.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/geyhtyfgh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gsfvrdneg.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gcqlvltzp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gvwwopniu.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gjoljxwzk.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gppudrmtz.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gcvzijcot.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gcjkcrvhj.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gykcsfxfs.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gchrsftlc.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gtqlxstoz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gxiwiicqm.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gaiqncekv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gzrqnzmnb.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gmojruggc.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/goguzwrlq.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/geqfndsea.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gvlizdzlc.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/ghuedcysi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gipzhfpsx.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gadzvaahr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gvvxbajjv.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gqwqihncv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gbgarvpkt.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/giicsairl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gnvrtrshq.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gkjjianhv.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gmqsvsrsy.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gtmmoagfd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gyjtaxgej.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gqedbiyen.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/ggshyqrnd.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/grmplzszp.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gmqwhoakb.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gzpzromqh.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gdhgftzgc.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gvcgltxvf.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gpboqinze.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gzpvgqcda.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gxdddmwsn.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/grbbmwfpj.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gepfmvgfx.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gnfyqjafc.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gtzcspksg.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gyibwxzqr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/ggyqifqvr.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gcawqnqip.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gsfdrhzku.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/getmhuvhl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gmjssxwmz.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/guabkoxvm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/grvbyjyzs.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gsokrfryb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gvfhlujbh.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gjepcdgoa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gfuxswcqr.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gmwpavzrh.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gtyjjqmgu.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gqfeissck.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gadrubyoo.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gpmzffdur.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/ghrzviieq.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gnwsmyygv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gfcxbezdt.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/grlimafko.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gelqpdqsl.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gyywumzfo.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gavfxxaci.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gnxextlaw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/guaahfisw.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gprovkpei.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gnynrzphi.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gxjowivzx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gvrwgcyrh.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gqflhekvl.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gdpficruc.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gzodflpbt.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gairidkzw.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gglevfwry.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/guikimbqk.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/ggnlsvwnm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gsnlrfbit.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gkfceqzij.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gtnxnjkob.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gbrvdrpes.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gdlncwygw.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gahdmivke.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gzmdfivwy.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/ggjanisxq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/goidzvqky.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/goitoyong.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/guuvlmgaf.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gsesfihuv.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/ggyuxzphq.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gvxstybru.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gyzfrqvfc.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/ggzfhtipn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gydozzgge.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gicdpvspt.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gkusfghti.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/glnlarlum.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gpubvrbgg.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gxnukhcog.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gtkcikcct.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/guhuaqwnb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gplnlovfk.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/guclyubfe.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gopbpkeeh.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gzyklvhzt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gliteumfl.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gptxdtryn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gbpwgdtoa.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gflaobpfu.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/guapyscpz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnrtpnyya.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gjvlxnvzz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbflgpwhc.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gecureapo.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gyigrewea.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gpiipxchi.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gvwfulhiu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gxfjqglkf.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gfbtfhxww.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/giecurovw.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gijtvluyb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gkvoqdafg.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gfonxlkfj.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/glfctujdv.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/glzmzdguj.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gxuqwqvay.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/grsvqucpv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/guqbevgyy.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gmhsltopk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gopcdndyj.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gipxkvjxn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gztbvxouc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gbkupiafc.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gyaphlimt.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gigtbwtew.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gwfhzmdno.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gsuwzmekb.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/goyqbajwe.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/ggrqkecbt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gvllwomkf.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gpelbxqfk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gmirosein.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gkdzjeiid.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gjxlljmgc.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gkdcctyvl.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gujdhfksu.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gcawmfiaw.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gcsthuhnn.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gdteovlrc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gdgkpvlwh.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gtstcnonf.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gumjfsfbg.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gramzfrwk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gctlfedgl.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gwhnskcor.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/goocbdioj.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gsftgdtqd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gqzmvpfal.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gwqggclrx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gmcfaqwio.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/glxqaqzjv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gaxjldumf.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gpjdhqjhu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/ggbzjakbm.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gqeweppkp.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gtvxmuovd.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gczcxpyik.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gmnskcuqx.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/ggzbeqnfs.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gjipxcyce.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gcfxlinzk.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/girficgyd.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gcqfkljem.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gvsrhmeix.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/geomdtnys.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gguctqbmv.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gcjywrudp.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gmgtkuilp.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gbkvucjts.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gmmvdcpgw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/ghwzjqwjs.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gewlrqezj.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gbtcngxej.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/guzwnziuv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/ggfxppfow.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gfqshvupx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/goeompvaj.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gpwfbqgok.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gtpkaspcw.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gayifyxqx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gegwciuqj.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gtyxovryp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/godjyohcf.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gjbpminto.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gfafxkcgh.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/girvdzfgg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gjyevfddl.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/glbfhslxa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/guiawkbgm.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gbkoolacj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gqezsrggy.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gmppbfyqz.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/giforqrvg.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gbotystvo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gkqgzorar.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gafvckcos.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gdzsnrjvq.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gwqgvuihu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gijzwuilj.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gmgrjymtf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gmrktdavp.sHtML


<!-- 参考信息 -->