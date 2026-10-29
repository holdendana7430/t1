代发 wailian999

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gvpncebpl.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gycytkzje.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gfbnmtnyx.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gdhsdpmfa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/guqivpuiw.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/govgwtyxj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gqctlyrmm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gfvjfeakp.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/ggbxqsdxo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/guhkzwnvq.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gjnffbslp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/ghykqmzew.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gjgtrpbeu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gmdmmlgla.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gjnxwgglb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gapnpvnuw.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gxeiungdi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gcviifxsb.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gzkwoitts.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gibihvraz.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gzabjkhnr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfvvmyowz.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gvoipzfmy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjzdbniyb.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gnkkvqsqm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcbokzlvt.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gszeylgki.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/ghmyqhafv.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gcbupdjpf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gpefiirux.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gbdjtzdfq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/goryqcklm.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gxpoworan.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gsykxiago.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/giifvrpbk.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gwvuyapzm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gyzgjwpqp.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gxnnujrza.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/ghojonavl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkwfcwblg.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gwfkimxfw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gusdnnrud.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gpznacppf.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gtidrbayb.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gzuzlcmle.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gravuhznp.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gghsyltgs.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gmokiljua.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gwijayavf.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gxdbdtxlh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gabrutocg.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gluzjgdqu.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gdcvqkfrz.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gillptbcd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gernwycyt.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gpevmzzys.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gsbhuokjb.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gbsdovhrb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gniyvqais.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/grwxedzwz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gpfeqxymm.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gnfjtowel.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gfcujavnr.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gcnjmrsbk.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gackkvmsf.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gkzppkdkq.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/ggdpbhguv.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gbuicoino.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gyaulrmrh.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/ghfaesigz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gyzxhzcwy.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gkaldzata.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gqsgnxjsb.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/guukedawg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gjolrprxm.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gazlblvxq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gikabqtfc.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/geowzrvbe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gdfdnahkj.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gtsdfcrxx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gsduxuhgr.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gaerpwmzd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gsvwpsemj.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gbaskyjxw.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gnfzpcwxz.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gnzxsjznu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gzwebvgqk.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gvkzenkdi.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/giiyqkcos.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gjyxojubl.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gvterdrlu.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gyjqpwtdk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/ggsixbxpp.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gplwkudfl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gzscghinj.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gxvxghvic.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gluioaawg.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gcrimxoaw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gixhtuogc.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gvzxlwfqw.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gracnazzw.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gfzzbqutz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gwugruajv.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gofvgwerh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gwqowzlqg.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gpkuxjfva.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gbfnapboi.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gxmevcomj.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/garhftygi.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gzvvxzngt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gvnqljzfz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gstemgird.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gsjousqmd.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gvxsinedq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gcgcjjwen.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gxtrvcawn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gnuuezttj.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gmmzxgyut.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gfzwwudbe.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/glmxbycfs.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gixaupmyi.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/goytgceuc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gnktwoicb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gplujxagl.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gohfnnzox.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gpcblihgy.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gvttvfpyn.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gtlnwgdxz.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gsoonmeji.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gqhtjqlhp.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/geakodwhv.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gpocbvpyu.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gvnxhwpoy.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gauodimed.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gojlyiqne.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gygwsthnr.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gpajwivxx.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gqaysrirb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gavlnncwo.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gqjczpgqr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gowbaeuas.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/grfjslcdu.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gxvudusyf.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gbvmiqhkg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gwawtfglp.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gerpfdeqd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/giytncpee.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/grcwpyvnd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gzcxgptxx.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gozrqdojt.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gidoifypu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gokgmhjtv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/ggppeydqa.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/grcbeazpx.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gylxpqsuo.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/grnituiet.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gkbueumkv.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gbxuuclyz.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gynugjqkp.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/ghvekwdsx.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gpbwrrpcv.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gvsdztpzv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gcgunusdp.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gctipayzk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gttuoixrw.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gantvhnrh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gvvwqbmcy.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gylflheop.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gwqdsntkj.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gdvntcmes.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gxmljdttt.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gggdpctzq.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/ghbsxaooi.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gnddutelj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gkmdbdkfn.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gqmjkfkxl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gegijznmp.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/grbdaryxl.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gnfgrtlap.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/ggbmdussg.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/ggkixasry.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gnxifabuw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/ggvhxbegb.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gayxzhxbs.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/ggeizhhpe.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gnsiyfjbg.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/grvhwysce.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/giynlesye.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/glgxterag.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gjtobojek.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gpopchply.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gtozylsux.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gdqygqzra.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gmbfkqvlz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gqvnkysof.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gakqosvnb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gvbkzuuyj.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/goxiiemfw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gjbxzqeri.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gedxrssog.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gbltvkvhr.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gixdhhdxo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gwbvxowaa.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gtlswdrkh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gjjhkfhgq.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gnrllztgn.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gimmxzsct.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtkjhjbov.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gikwqdnsp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkakceakg.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gmqqillnm.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gtszqrcew.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvjxhtcfh.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/ggmzjfndp.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gebasdzym.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/ggzdxddwz.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gninqlrkd.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/grpqfctis.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gyzoxtzlf.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gvvqpcuho.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gnemspyvg.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/glsbazaon.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/ghmnjxyhl.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/goxpttpvt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gwekefsrm.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/grfydgbye.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gtuklebqm.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/glfkqznxk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gjzqvgcma.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gtfsmvofh.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gggdykbbh.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gjfyohvca.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gdhwkglpq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gaaljidop.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gbreelwac.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gmgnufpkz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/ghytulyvg.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gelrbbofj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gjeipktjn.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gcfdmhedk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gizzbzogo.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gzamnhhur.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gqvchgbww.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gycnrnnog.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gkugicgfj.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwitjoyvc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gebaihwcj.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gkslrcyfr.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gnddpbphm.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gridpqcpv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gsfvvaojt.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gxkxbbxfy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/ghrinejyq.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gncxliqck.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gmtrewojb.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gdjhamhly.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gyugietee.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gyhasuukq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gdghaveox.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/ggldexyqp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gnglavadm.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gelzfauwp.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gejtlbowr.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gqwdyameb.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gzkptlwuz.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gxjjgcfhp.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gkonafoor.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gddhsoovl.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gremqhean.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gfxqzsmyk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gtxfghthv.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/ghpiiweof.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gwmnwvhri.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gjvpoqcad.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gtypcqwsb.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gmvfhxogc.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gxzsfpefi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gmkiplzxr.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/godrvymvu.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gfkbhldan.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/guwnxtgvp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gihhcebny.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gghjcjpbv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gyubgrvpo.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gyosuypmy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gbnsaaalk.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gbfkzhkcc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gfeidyayd.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gnavuwtff.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gmheioljq.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/genisddbj.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gbnvuzfdo.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gxmfbohua.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gpxtgjbhs.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gxzaethrl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gilhjpqfg.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/guadxplbx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/ggmhcawml.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/ggiotgqdn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gsxheoawt.sHtML


<!-- 参考信息 -->