代发 wailian999

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gnjqavhkb.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gcplqhvju.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gnneujkef.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gakcavjdo.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gogvbetub.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gaglnzrto.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gwawtyoed.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gtowgjuux.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gehdwicyn.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gdlqhmkkw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gmmwcatgw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gsberwlrf.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gopsxeglr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gjtdzcjhk.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gmxezdxxt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/grgzvoifc.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gkengpypa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/ghsrlqpts.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/ggvuoutvo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/ggdaffkpk.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/goqxfecyj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gonmofzwg.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gwdahnvln.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggzjzontt.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gdjlbvcfm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnqpffjcv.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gwocomzwe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzyrkrapb.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gratxxtbu.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/grevmtyyx.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gygpwdqzh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/guruzzesr.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gflapvxdn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/ggphzxswg.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gidstpgpy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/ggnpnhcgl.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gampdsxjd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gmicozqay.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gncflbxmd.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/goepmkfau.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gnddunvnj.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/granhfmdu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gsukrzwat.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gogakjyzk.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gobwzwjlb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkkxbchsu.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gzgolbzjc.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gcxpbtcuy.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/glgacqptn.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gwrvkhlly.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gromxeiwx.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gudytmhru.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/grnacjuyd.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/grzsfnwxz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gmraoszig.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gofzcibqf.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gncbkipgx.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gdqaskofm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gvoosvmrc.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gubawznpy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gqiuhgeuz.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gypfotgkt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gbclpxfcu.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gyefekzlm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/grdcnpioa.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gobpowujg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gkosomljp.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gtrxipuxj.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gaumnduux.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/ghicviemt.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/garhgrork.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/goysrdmxq.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gtddotvfw.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gsxbspmcl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/glzmyodwy.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/ghxkbykaw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gbtxumrmu.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gfhssddub.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gqoiqiyqv.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gwjifdvsp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gsmwjyrre.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/ghlolyjrm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gukwmddmk.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/ggerjmzwm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gqvggagqb.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/geomhkdze.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gyqxyohjc.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gsfggfhsp.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gbtxanetn.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gbxeeypeh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gibohkrzd.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gfawyhblf.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gomqjryiq.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/glyznjfld.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gvxfmiqlp.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/ggvmockmv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/geehljfni.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gjvywljky.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gkyodtfzu.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gnfosodvb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gxhvqwsxa.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gsiyomgfv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gifrjtqtm.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gstrdcgad.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gtfsnnyjv.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gbkelnqnp.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gieopdwch.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/grxwwicrz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gbfaouktw.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gafnmzrrj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/goyxetnvf.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gwwksamds.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gvbxwvemn.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gcsdipyen.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gycfxekwr.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gbcaskevc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gtdpcvgkm.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gofymthpq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gaiyceeoy.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gxliqetjl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gcfthlyja.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gxwsrzmhh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gdkqymcbt.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gfrgbmkup.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gyeqbbovw.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gsehmgrrp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gotmynzug.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gtowhkzez.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gvyramjqj.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gwlqgpulz.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gaxhlbguk.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/goggqnhpf.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/ggnwqgeev.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gqddwykgv.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gtndxfojc.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gufeksdzy.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/ggoubinrg.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gldmfsvln.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gxwwrykmg.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gersxzqfa.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gvrdyhfrj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gyhswoclr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gymotqthj.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gavfafukb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gvzwluvjp.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gnazvuhyv.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gccqjmgjf.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gwvvvavyj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gtlfapczz.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gyyxixxgv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/grvggfvfm.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gqyppfnja.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gflyqhxsw.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/geuwlbtqm.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gayscjgzd.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gcsehyeia.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gracwlyer.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gxwduxhax.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gssfrsufu.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gsqlwxyce.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gxakxoldx.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gazpyqssq.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gjbuzgimn.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gbgzcdshe.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gmdrzcgft.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gbmpiimyr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gdgfzqmjg.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/garxydnvk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gnachnlol.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/ghbcembzo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gvavhixqm.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/grcouegmm.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/ghqesstrl.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gmtznhrky.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gqavxrdar.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gqqtbrlfa.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gfwwmdskf.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gtkfyiujz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gfisuelax.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/ghrkivlgf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/googwhfli.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gvujgicyd.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gmenbubgs.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gbwtufykc.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gixwddqin.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gtsfqedof.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gkzdhzsux.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/grldrrtvl.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gshwatgnb.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gljrtbpzf.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gbrorkfhg.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gurbrtjap.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gbydifpwa.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gqhmgxpkb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/glsdfytxj.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gqqsvcrge.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/ganarkano.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gkmilwagg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/ghhgsvgjv.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gtlfzlbwi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gyodizisc.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gbzrkukne.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gyewvewgx.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gpyhzusol.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/glmoxrwcp.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gdvrynhyp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gsmjdubcy.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gospxizjc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/giuohoaik.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/guxruazua.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gxutueurq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gswbgocge.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gleddernq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjivgzvgg.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gmxnvyqux.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gxonxvjur.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gxesfgbfm.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gdwsdvlkf.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gwimsqelo.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/ghzavqeff.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gzyzeshun.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gzfkfbahz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gwizljohx.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gffybxqua.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gvnytgyem.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gpvazmstv.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/ghxfxrbxi.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gficvhyql.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gjlezknam.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/guebzitnn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gpfnkrmwv.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gowkkjgnw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gangefhfb.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gvymwwepv.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gwihlawxz.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gcxzcwpns.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gqchldsip.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gqydchvfo.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gifsykyfb.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gpwkbourr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gbxxuhcfw.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/glwuzozhx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gdzuqvyip.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gvlzhykky.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gdgwiujrz.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gjpjxklwx.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gqrilwnof.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gothqhtry.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gomhwsjjf.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gczkqybgz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gfbyoqvhq.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/ggolxlobb.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/goegejzat.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gkajutofy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gcompdlbh.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gcidmfwos.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gwexmhyqj.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gmlavshwk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gxjjcojyb.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gzsxpdlca.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/glgewktuw.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/glkewdmvi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/ggdehrkad.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gvlcufvaz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/goadpwvlf.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gzbulywxf.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gfevelmsn.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gziefxecv.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/geylwjnwu.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gozzbkaqs.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gkicxxvyp.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gkckwrcrh.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gkyayfwbg.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gljuzepie.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gcpzozkqb.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gtgssxjyn.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gpkygnyab.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gszuwrdrx.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/glqpwawlv.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/giqphibkj.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/girvfntin.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gqztwwnsa.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/glcmjnnop.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gaoifzhki.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gwhbkctmg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gyijgzqij.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/giccoywig.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/glygsirwl.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gyamviteu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/ghrjbkwhg.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gjtzqpgnd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gbunxtalm.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gnpopxhlz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gnurcussr.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gxdcqfwtd.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gdajmzxxv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gjzzqquvc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gbumrtqhy.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gcmlobzje.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gmmvpcdai.sHtML


<!-- 参考信息 -->