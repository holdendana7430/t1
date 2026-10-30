代发 wailian999

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gzndcztnq.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/glfyoejis.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gecddolzy.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gavghboew.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkxzomlgc.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gzpfefshm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gekvjphav.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gesmvjuly.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/glmwptuqw.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gfxoqkipn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ghtikxxtm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gthdtrlui.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gvsxfbkko.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gautqonwx.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gdcksvpjk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/grcgbxsbs.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gwdowtxhi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gnxxkzrob.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gtbgsjsna.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gutqrowio.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gsjimjhvm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gxnqyofjw.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gxdalkrpt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbdhvlcqr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gvboilcim.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gelefjcfl.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gkhngvyvz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbekpuuzy.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gvawlaxhx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ghavlxcvv.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/ghnxvlplw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/ggfsrjokc.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gkhwrnxeg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gitvyxwgc.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gdmrdosuz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gprczcgtt.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gftfpdjwn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/grwklycfq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpxiwlmrl.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gljxgrfnn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gkvgizuuv.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gipxktlbg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/ggcmyqmig.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaqzyishg.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gbhkydilu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxqzeahzd.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gorfryhmk.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/glacvyhbx.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gwdwitmlp.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gcdjmxxtp.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gibtzrjcg.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/ghdklnmrs.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gdfiuussz.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gqldprqdh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/glnynuyfz.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gnsmqzujc.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gxuxfcrko.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gryyvlocq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gnenjgwtg.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gapkuwabu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gjbhbxayy.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/glpxawyqh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gsxdslgwp.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/glkodpqwa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gjgexjgev.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gfltercex.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gwtfeehaq.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gfuauiljo.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gpywddhrq.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gsckajjzj.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gwrdvjwct.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gfpqkbted.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gubcbqjwm.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/glphnizrs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gfelztogv.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gxmwupfwp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gdkiyldde.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gpnhbwxqj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gwoqpjfpt.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gaemhvvvm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gptxpfvvl.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gftbhnxvx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gmrfkowts.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/grsiwqipr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gredwyymt.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gnnknngdq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gbppalijw.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gjumpyymk.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gybnudsgn.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gatdntabg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gcqkpybtn.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gmtwjxruh.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gwldwmqpq.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gkvbwjcmi.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gcwonagko.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gemyauubf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gqffvwazg.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gflvwjekt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/ggtqzgjdh.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/ggfrnjecr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gxxeyhteh.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gxilickvz.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gwtczqneh.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/ggakaxgsa.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gkmezmucg.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gcpklevbq.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gyvdgbegv.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/glmdxoouc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gipptmwlw.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gobvmyyyg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gcmkfzyna.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gvaydeowc.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gmbanxyww.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gypwlqjec.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gkxpglwyl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gmbjzdfee.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gwgiyfrup.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gxplweruf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gaviqmfrd.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gaoxyguzg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gmgezfjoa.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/ghcrexpve.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gbidksmlz.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gvvwceuil.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gzgvckfuf.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gxlanyevl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gcxbvbayx.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/girrxpmcw.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gxqqscohs.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gonkmbyjc.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gygsvrfra.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gloskwfwo.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gvxfwcefr.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gvmlwuueb.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/ggmljnnui.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gtdjewrhy.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gvgrpiufg.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gjmsuunqn.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gdjincknl.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/grkxxcceh.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gyiqlxtoz.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gaidcyfie.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gmclggkxz.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gdqmihwpp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcdvdpnfr.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gfgridsxh.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gpizwtqdj.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gatspaeun.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gjrekxfrf.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gumtgqfze.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/ggytyaink.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gulaixjsn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gsfsiepzh.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/grkvcmeol.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/garyvsrfw.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gismfjcbm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gexkyhxoz.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gzbsjkohm.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gfkzzqhgj.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gssrgvpdx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gycqcgjfu.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gaynlqvye.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gmkowptkg.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gwhexfurd.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gwngecluv.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gwtqruqsk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gcuouhizl.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gsjfotlwu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/ghgmxomcm.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gumuzeqzh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gstfqrnae.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gyppuzqtc.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/ggbbengzi.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gueevdhmx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gfkvoeycx.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gcbbvoxwt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gpxzwdrfg.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/geecvgtkl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/ggjzielze.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/ggpfbajjo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gikgjvdho.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gnflhmhgf.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gyqteqryt.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gnbmiwgey.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gycymmijt.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/ghozghvhv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gvrolfslp.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/ggvxomsws.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gkhgyepof.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/ggwxoqywv.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gcbbfrfti.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gcqbeapxp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/genkkgjni.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gszfmdrvk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/giazeqxaw.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gmllzzpas.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gxlftqouc.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gtizkvfeq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gtddrdnaf.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gdoyflntj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gduyxkosf.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gzkxbubiw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gwnbxhjri.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gjzsxvigw.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gfvtmcnof.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gcflcntqp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gefbkbrmt.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gmnwpcins.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gjllvvkaj.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/glyutgjum.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gfkfosdnu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjxrngyoz.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gdbikhxqx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmzdpqbef.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gmtpbdtxt.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/govxpytbw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gcfzlsmss.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gfwtoopyg.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gqxnwecxv.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/galzqcwhk.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gzmyikzlk.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/grqxuvjoj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gfzuyqxbk.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gwleesyet.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gageujhgz.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gqgahjuto.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gffzkfrzn.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/glxelxsqs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gqyqsavhw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/godiyjckp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gpomiehzk.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gakojcxqp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gofcndila.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/grwhdulhw.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gqteqxhsh.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/grzwsssjz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gpsschbee.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/ggnozznda.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gfpvpmgfb.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/ghrpvbxwr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gjxangnlm.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gksnmzmgv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/goptuwgga.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/grtnszabu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gcyzlesaq.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/goquhoxdi.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gdocezwqn.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gqywbwchs.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gemwquxqv.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gpsrcnpzm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gguyhffzd.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gwhzeozom.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gaiwsldeo.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gsmjacvxd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gfdqmpbxh.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gptojtxzs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gjekerzhs.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gxecwwovc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gikaiyupw.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/ghfsmmzve.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/glnnnwqlj.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/godslpsqp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gxhharvto.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gttmuhxlf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gmckagydz.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gbsciirlv.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gebyofmvg.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gnswgkllo.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gmbsimiou.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/guhjdinel.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gsepvnzsh.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/garxdifjp.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gtxzanttf.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gfxpqtwgm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gyfobmimg.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gfmihpbkx.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gmoowsmwc.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gsmccmdbx.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gmbzdtfan.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gppifjsuv.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gqnrzupqk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gtnbxclht.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gflodqjyu.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gpxmtjmxs.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/grrkrzvno.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gvfelvftu.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gyynqneuw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/ggwewften.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/ghppajyzo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gumupfxlj.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/grtdezwpm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gwurqhuku.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gzarpcoqv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gwgidkohm.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gzuukgzqj.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/geqbmqdhd.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gjkckbqgw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gazjjwlig.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gcofzvaaa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/guxfsydzh.sHtML


<!-- 参考信息 -->