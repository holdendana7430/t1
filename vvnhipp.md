代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqqpwmdp.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gzmmfejqn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghykfhpjh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuavlwzy.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/ghcecjrkb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gjigotxdo.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gesyjbbyz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqamrpgmd.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gltviopaw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkenjkrr.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gfsqkdqax.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gpihecrii.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjzghcgr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwglxxng.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gxczbtqwt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwdqmufb.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlqfucnu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gupcdcemb.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwkcmcso.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkapnwrll.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/goxfnyvvz.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtndgafqm.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gruifnvjd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjvjhofs.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdrfahva.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/galmwabjb.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gqvjfzqkv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gybafkaxt.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzarlahcy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnkdtwng.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbipcutea.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gpqtymjye.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/garueovdk.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gdlkziyql.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/glsokaufu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkrvqjqgy.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gunkqhbgl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcarpqixs.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/glkhvvvsj.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gwptkdjlo.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gupbhtlxw.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gnelfjkcv.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfbmesvl.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxylhwswk.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcoughez.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/giivkvqxu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkolciju.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gupjwsgxx.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpbpglwjt.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpbpfccm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkozjnyhi.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdewshlht.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gdppwpvsd.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gngzqthke.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/guyzopzhe.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrbhtgbw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/grlosfgoh.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gexhtfspe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gugmmfxxk.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gituggooc.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpeulozw.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbbqazec.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkilvldz.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmrmltdx.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gpacmsmwb.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gsedmosaw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnbejfahm.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrynqukw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghswuyoej.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkgugdfq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnycblobk.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gipbnocdt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqedpromb.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrwzxnhw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/grpfegymm.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfdjflvm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gomayegxt.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/goyybodkk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrglufya.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gplyssdxa.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsyrnauu.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gecdfbvfi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gunhzamkp.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gbqhbuhrp.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcodgcqu.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gngfaciht.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/guhbkcmmk.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gshvgopls.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gyslwgbos.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiicvnyn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjtiborkv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gieobsghm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevmdgemg.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghousldaz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicirhwjv.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gelahswfe.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtddshyzn.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gxdhrijdz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoznnroo.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhgciwsm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxhhpppg.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gnqilnuni.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gohgxdidh.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gqitgbqtw.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glaonzzbc.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gewuzvxwo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbysozlfh.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gjpqtryab.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gcahysory.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gehbvjhcd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaooryyk.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpdgnxqp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/glggvjnon.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/glvyyjmbg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/guljbdxpm.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gthctgvux.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzxboocs.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqjvnibu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gslkiszne.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gtozwtojy.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gagsshxiz.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gygffncvr.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/ggoozhuyn.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwczmpetf.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gxadmehqy.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyqvjzum.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjcpmelzr.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnqvkwnuf.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gvbwadupr.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gdshlisol.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/guibgybho.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/goegbrqsl.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoeosozg.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gyuqckvpa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfgjvnrk.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrecmuvg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzboxwuks.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gebuyaksb.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnnzgukhe.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gaazikazk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gsgluzoay.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/guanyakfh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdlpubva.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/glkljhgep.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gboqnpbck.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gnpjfrywp.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gmfbjmpaq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqlrsylw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gcmsbjqvu.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggwkcskvl.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkuvpbydx.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuyutnct.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiqezmbc.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwygfajbt.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gwztwqjqd.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gxewklyen.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtruqgaz.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjdgxawi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gzpzbfpze.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gamjrorkc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgjgiszu.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gmemeuytk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gknniaczh.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghesghvai.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwilroazf.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfudtfrxa.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gpqtpnkcv.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/grgteilzw.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/ggayjlutm.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gavzcpvhp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdahjdqyk.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gecxtpmfn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaefxbulo.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gdsrkmkud.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gathivpna.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gmojoiiek.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpilldfkf.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnghjlsei.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsmqwltco.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyghmutgh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuftbmmu.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyibrwnf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujppjlsp.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gfeeewpgw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/glcrjorml.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqicxrzg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsniidqu.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gedwwhfsh.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gdubvebjx.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpbutbpz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gudlzzxou.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gesaefnvh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnqslojd.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggdjdwhcy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gdanhyojf.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gdaonjbsd.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnuediqc.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/grczxjjzk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejuivdnr.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/ggxzrdwqw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkebdruky.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/guvijrqat.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gpsnyfxkh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guycruyeb.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwxhmxno.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glmtqvqrs.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywowhlxp.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsvepsir.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggttqlfcb.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gxwiiqikv.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/giyzgrmfc.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjngfbhbr.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gdvgistmj.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdojxzftt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxnwsrim.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnuoxjwu.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gthjcpkax.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtquhvhcx.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqnjdorh.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gnfwaetgc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gkcrafkub.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gcasvvmqj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywdstzoy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnlkvfty.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaqosnxz.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/ghbqmhlqt.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaorfdoen.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcjpjxqid.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giieimzdp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gmzmhtddo.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gmsalmmdp.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqsjgfazu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrnslxkf.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gvsqoorxb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gqnrjzbxy.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gdpjuhdpw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gjernqthr.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpxxwfyq.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gycyifikv.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjjydror.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzzvjfvg.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduzwtmaa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/ggyzjbebo.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkjwtrqh.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gklvuflqp.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzttdyinh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gobooscvb.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/ggijtbmfl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/geohcpoln.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gxglxzgrg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkivhnic.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowutmgiy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/godmeyugm.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gowwiczvm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gtvmddohv.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqplwvpy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gjvpoeuwj.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gfkmbtebu.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gayjumksf.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnlgpsba.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gahbktahh.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gxbjomzxs.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqskfdua.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gyeyujifd.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvloxuylj.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrobqdke.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gquoiuddi.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gqczhsoso.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galizzjhr.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/guftakyuj.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhzaawgb.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ggxrmodsp.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuomygtv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljmpeatb.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gggfuhlnx.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gigopotbk.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gzcgzuuti.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscndzqri.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gptmbtrqj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gczfuvdoj.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzitkqpz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gdrkawcsd.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gneyqbefo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaedjdfl.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzsqvjmy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzledjzfu.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gxalqjvuf.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gogwuqskv.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzkdpqbu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gunxsvzzo.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluovzvsq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbigbfxxb.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwplijzao.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhrtajib.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/goohqomwa.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gikxhrlby.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/grfngyxop.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gryumygts.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gaifkkyud.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtxaakdck.sHtML


<!-- 参考信息 -->