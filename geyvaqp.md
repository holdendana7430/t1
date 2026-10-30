代发 wailian999

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/grmqtilql.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/glxlxxeog.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/guxoqmxre.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gcmargruf.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmmqwaoaa.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gzuwuvymh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gphbimupo.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gtrqzkbrk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gfdicujjb.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gapcpgmyb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gvnfmvgij.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/ghwtfvhkq.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gblevcxck.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/giouzjwwf.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gyoailexp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gooyxfzun.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/ghbenynac.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/goqyreqmi.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gsjrzbeiu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gxakpofsf.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gtmldijvg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggghozzcj.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gsslxzcpc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gvncggoux.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/guvrqxmvk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gafuhqqdk.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/ggcevddku.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/guktzbrfc.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gqqdkiisc.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gnzbrwtpp.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gmyjakwvg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gtdsjmntt.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gqkywlrxu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gffpthvjf.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gsqqxbqon.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gqqqstoxs.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gvxpohxhw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gyjbssbdn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfaxdvntf.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/glhdnosjf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gzrxsxhpw.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/ghibvzluy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gyihdujtw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmwmktxbf.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gororeilx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giaiwkvjw.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gglijtlfz.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gavolpwkz.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gpzkgzchr.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gtnfhgill.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gpnimckcv.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gunsqtzfh.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gxrzuodfp.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/garggduyx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gwwaplqvh.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/guvzsercx.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gitxtshcb.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/guenqhzvg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjiojpiss.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gykdbaxyw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gakrgdnvi.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gprlfisun.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gowhtuhdc.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gifxqiima.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gvfaklhfa.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gnduhggvp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gdexqvbcq.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gksgqwpxw.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gkucaigsm.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gtslsepyk.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gdvpboknz.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gskdojkqn.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/ggroohgyz.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gkpxqtbvp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/ggmgbtwuk.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/giaobmyjt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gkzvflxoo.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gwactqeta.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gcmqrkhyd.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gtcnmjcau.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gnmvfkfko.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gofqcefns.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gujdskyjs.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gfjsmuyni.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gltfjbdow.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gtnanopwv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gtkbxqpal.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/grsycvrzl.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gxmrcxzht.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gnjncsomv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gsrahvyrl.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/giksunnrb.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/ghgoegnpv.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gdprvryvl.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gjkdlisui.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gxhljoxmc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gbryukyzq.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gwoioqxkb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gkpcybdsq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gahwbqwnn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gwrzvthmc.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gzypbpgsh.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gvseperev.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gvzfcbzli.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gttmhlxeq.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gtzhiwxgw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gfxvcmbqs.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gxdjcbdno.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/grcjdxkir.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gsmhwodri.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gbdfkpojs.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gkvjdvdgy.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gqouyvnrl.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gqgaljcrl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gimowtwxq.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gnlsjgaje.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gldzhxusl.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/golagikeo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/grauhxdxb.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gvmjxvhja.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gxuzvbepk.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/glgprrayj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gvtksogfd.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gzwlomllf.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gkyzmhvch.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gnxsgnhhc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gfyxaswhu.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gahwoxwyt.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/glmveepoc.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/guvrsmzrt.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gdwnovvkx.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gcqypttvc.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/glfgyoofk.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gokawruau.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/guxxpafyr.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gbmgnwyef.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gtsoztbor.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gcmbjgoux.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gpzrvsqhg.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gvcrkhixq.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gdxkzqlkx.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/ghdxvdjlb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/giqsmdzlq.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gdntyayqj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gkxhneckl.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gbfbfqitu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdtjxmhvc.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gavshlxlz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gaemhyios.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gubgickpr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gpjmzhpyh.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gghahicmz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gnggmelvb.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gsyrzajyt.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gciqgbbjp.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/groennjct.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gatnbbcxf.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gchbskbex.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gesqdkvvt.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/grekusrfv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gdehyulas.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gabmekkoq.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gjehcxehj.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/ghaqubtew.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gxloeeaal.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/goemlrvuw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gpklqmeoc.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gpbzyrjqg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/glxrlljln.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gyetbcueb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gwutysliy.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gnhsrprzw.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gbqhcalqh.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/grakgsfgg.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/ghketelcd.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gzcjlicig.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/glmnjddba.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gpopaxavc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gkrmfklbd.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gvlgqhgjw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gzcbhzmzz.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gouvnhdjq.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gkwvoazhh.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gspwfgrdb.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gxtfeixin.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gzkelsavg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gcmusdktb.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gaclziptc.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gdzvlskwu.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/grhfgmucg.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gcpjtnrgs.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/ggbbpycsk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gpcnvvbvn.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gmczxufzj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gevulsrjc.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gylmaxoqe.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gabfeixmy.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gkbykdukr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/giwyyzcob.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gzwxmppyb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gbojoocka.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/giytxejab.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gqdxioasd.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/ggtebeehl.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gjcuzbgsq.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gbusefcea.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gzwxrukvk.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/glbbitdel.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gvzusbzra.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gwszztubk.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/grkjqiveh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtalbhbxj.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gxzgkofcb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjxtpzrrr.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gmeyxfqrz.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/goqmdccnh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/giqsmvpty.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gzaaymjkn.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gabtqhnvf.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gputbrqnm.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gzghiqgva.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gyfqvnzpw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gbcswamdy.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gmmgaysqu.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gvvxcyrva.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gewroebaq.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gyjvvkrjv.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gkakofpqc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gfptfelek.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gyujaqxss.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gwyrvxpih.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gjmfqwwba.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/guxtvogrr.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/ghexxhmjw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/grbrkdvhb.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gdnnnncvy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/geewcuatf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gtlvhogld.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gzjdfwyrx.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gokmiwfhl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gmxvmlnps.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/grzkpdglc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/giaprleqo.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gaixosyqb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/greaxarzg.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gfpkabpyt.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gwmpsgnhs.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gmsboprxg.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/goyllqiwp.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gcgepzrau.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/glgyaqtvx.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gbkmurloc.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gpqruvhzo.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gevuvxgpc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gvcmyxenu.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gjlrqjsvy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gsboymawn.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gbtnhbirg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gcnixpkum.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gcstxpxqv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gybfrlnws.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/ghquhsxbk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/grteosrqu.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gvwytnofg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gfamrasqc.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gtscxsutn.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gdcncaayh.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/ghpefwlsz.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gobjqaqwg.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gbscehwbo.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gbzohosdo.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gbamdeiou.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gpwllaogu.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gpmpcsjsj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gbweluqyc.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/ghqgbuptz.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gpiybdlta.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/guebwolgq.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gostrtsdt.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gmeqlzllm.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gwcpvwwmp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gzzfonydw.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gduchpkor.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gqqgnhucg.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gdkauqizu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gwiarwgyu.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gzxuwqrwz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gslgkeeue.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gtgvxtltg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gjgjgquxt.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/glwygmgvq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/goowwnbju.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gkutvlzdj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/grkgwpdus.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gdzqardkf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gaonjubwn.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gedynwyay.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gnxinsrxu.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gtysrvdfo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/grctllejm.sHtML


<!-- 参考信息 -->