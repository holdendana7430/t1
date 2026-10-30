代发 wailian999

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gbupjgwyg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gwqohvgsc.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/goykuiaab.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/ggbghbwbl.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gvsmywwhi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gakqnewcr.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/goemahsgw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gcvznjwrd.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gsgqtgldy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gavoyfujt.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gthyytjoc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grgkafngp.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gosmqacfe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glkhvuqac.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gimllvxrl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gybbojceh.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/garjfvkfh.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpnyiafnh.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gdogykvuf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gvihpdqfj.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gvfwnoivb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gvksgixyx.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gmaxrluck.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gcmmifjwl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gmozwbeow.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gedfktghu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gohyjpxep.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gxexnfmkn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gbveowbav.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gernargkb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gzwjkpqjk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxzjwvwpr.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gavfnkxwe.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gegcjzikf.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gmfpxafsd.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/govjnmbll.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gcwlhtzdd.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/glatapxim.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gnscwspkj.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gcpsigolj.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gyxhwpojk.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gkpqgdwyy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gysktzvyh.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gjbhcxswn.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gwsbxbrji.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gtbalumki.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gbhctukto.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/guodgsqzg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gylzqzdor.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gkdaqwfss.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gthnrcasj.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gykfuobct.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gsjbhrsoh.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gxqgouemg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gcgdmlard.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gbcurvkcy.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gwzvlcvgn.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/godfqjyvd.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/ghblqethf.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gexfysvev.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gcesrcnzg.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gnpouduoi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gozgekhvb.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/ghomwwzml.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gavusntkq.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gkdfgysyr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gdqoucsfc.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gnereqlet.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/grazaqpno.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gsvtfbfpf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gutigtbkv.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gznigbosg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gpbokuxow.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gtkpjvqhx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/ggkejnbmk.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gckuslfeu.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gifqjpprq.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gzwlsiywr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gpjtifwev.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/ghyxnoqpr.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gvwfposjt.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gdggfoovf.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gelwzmxam.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gwoyzyxpi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gjtyaycgy.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gqgjypugp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/ghkeqmjdy.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gghdzjcqi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gezlqfvfi.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gatacajoi.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gidjihddp.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gzwacdosp.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gugtivyhr.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/ghubhixjf.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gxckdzcge.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/ggukhtwuy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/giygvzisk.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/goavatfiq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gghhpghow.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gqenembbw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gqbvrjwbx.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gtiljvzhy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gbqflyxrk.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/guczqxbtx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gmkplddfj.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gfnzuwzqp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gyyooczdu.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gavngwhat.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/glweqblrr.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/ghfmozbqp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gzbscjnqh.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gmlaldama.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gzyumuicw.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gfrefqibn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gzdncpxut.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gncxduois.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gfudhnizf.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gsbswgqgx.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/ggloqueax.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gqcsyfvko.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gjmgcbdoh.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gpohjbaeu.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/goxwkahss.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gnxmauivu.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gnsbgtgug.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gqsxbfolq.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gpotlivme.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gowdawoco.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/genriphef.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gxzrecplt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/glpygjhnx.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gykqjhogf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gfbwdtepr.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gffetsvuz.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gkkfqixod.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gevnqvbgz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gkdyzfznn.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gucysdfey.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gyppjktts.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gtbjnywhg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/ghpizrgkl.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/ggnjehugs.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/godtpyeoo.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gezpcnjcu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gpuirxani.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/grpddukcx.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gevfebelz.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/geftxpzgi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gkwekqhih.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/glimjscwd.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gipdntnlc.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gcshyzxff.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/goqceyppo.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gywhiponm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gckjsdhvk.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gzdvzdwlp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/ghdhkumsa.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gznjaithj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gycrredws.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gpdawvljf.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gpegofnhe.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/grvkupcxw.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gaeonguqx.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gbgiqqtel.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gwqydsdnn.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/giotcjlhm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gfsxirinm.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gpjemdrra.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gccklfykp.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gjebubuyn.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gjfpjjzzi.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gqtxclsmz.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gjqhoemfi.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/ghtrgewuy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/grayigdyw.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gdgknnsmw.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/ggcxweuod.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gzopugkob.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gttxyhroe.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gvuvvaryr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gguhslqkg.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gvepaucfh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gedpguxhq.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/glggfslvq.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gsycawmhr.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gkuzjrbvu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gzzfncgcc.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gvvixhjwp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gfbulrzde.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gnwsmefrk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/ggweohcwd.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gyfddxotx.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gfpqcmxyb.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gcbqpzfqd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gkrdadggb.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/getnokeer.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gpnbzrrvc.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gdgswwbxq.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/glhzbfatc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzuwmrbia.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gvtodciax.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geurfblkv.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gskikuakj.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/grylufvza.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gimtrpysd.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/ggvgysazj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gghjsdpnv.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/ggbqbphbw.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gtnputktf.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gmwxusuyn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gljcyoxqn.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gjuxwcloo.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/grrdtmtiy.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gusboxscx.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gmgjambip.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gdvoxrrmo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gbrgtlhor.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gevvehsev.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gycocsnlf.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gvxwkvmeo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gdlbmagxj.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gjcfskmyx.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/giefkpyow.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gjenvtgfs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gswfjsowj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/guxzizixw.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gjcazmtfy.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gfgwenael.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/grgzpvudt.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gwsngylnv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gdguoxzta.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gpfpuqkii.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gvhnxkbzv.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gofdwbrln.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gzjyialpz.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gvlczyuij.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gymzdjgci.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gqcnfmoio.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/glfelsqhx.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gwioagivp.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/giuuobnng.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gqoifpirf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gaxanswlm.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gnnfnmyny.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gsqelxpuh.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gbsogmprl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/ggqogjiyx.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gytdhvsev.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/geeqnvkqc.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gbocmxpkn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gjjfpcczd.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gwytmxbap.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/grbmfmmlu.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/grnjmzoci.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gxnssuvog.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gwvvxftyc.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/glkombhrb.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gffdtmgmp.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gqldxxxte.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/glcotkylv.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/ggtdtfnja.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gddobtvbz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gzgautdos.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gwtmtubwn.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gildjjkzv.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gsvfvpfxw.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gllsjwulr.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gssfogocv.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gexaaccbw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/ggslqkdeb.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/grmnflhcd.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gnlglipje.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gzbwmwkzi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gbqinpgis.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gklfnyuyq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/geyqgnhal.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gxrnvszro.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/goxllaiqo.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gdszzmaiw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/geshyaqqu.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gursppfbc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gqfydrmce.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gdwawdgzw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/glpnlkpjj.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gzdiurapr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gcvjlruib.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gcbfjugbn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gpdndtppw.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/geblmtbjy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gyxieggxe.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gbtkycpkk.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gulttjpmf.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gqtfysvay.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gvtracaae.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gxunhcmlw.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gqhhdbtzm.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gajmerngv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gzlhtrhmv.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gmppfgrsr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvelzipfk.sHtML


<!-- 参考信息 -->