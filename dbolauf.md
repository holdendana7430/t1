代发 wailian999

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/glhlvtrpy.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/ggutkvtrm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gwhldwcjw.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gjqqvwihl.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gausjjynn.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gogltzswo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gvyrqspiz.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/glbluvejp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gaimjodoo.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gwqwfumkj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gknrlbxoh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gzkvfgvcv.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gnrdyrgtf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gmhruttue.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gtkdbvaxv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gdlwmmfqd.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gygvedeik.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gekhwknym.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gbhwacioa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gkpenxxyj.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gkfixoewb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnmlwjhkt.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gqozjbyib.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gyubbgzvp.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gcvdegagl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guhjebugq.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gtvbyrtlq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gedfiaywe.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gesmkddpk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnpfnasbi.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gbbjevexs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gljsbnjjw.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gjdlpjdbl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gfzixvwla.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/grgevrfkw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gmipyezok.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/ghdqmbqxh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gptfwsibf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdzlepxyn.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gsdblwfnv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gizfprakp.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gcefrulaq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gkjbttmvh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbydfafws.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gmykbixvm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghrozmtgg.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gxbzgivat.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gtzjxlzdw.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gmiclzoov.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gcukhqmru.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/ggksglkav.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gdhlhscnr.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gzlvagnqu.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/glwrdqpei.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gxkaizmpo.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/grpvcxcqs.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/ghqwopnpl.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gnvdjgntt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gnawkyuqw.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gdtnpmgvk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gbxhjkhbf.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gsecnyekg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gyarpadkn.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gdpdajfpg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gbtktneqc.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gklyokjba.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/ghdfpsnvr.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gpexqyokk.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gaygxhsqv.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/golrtnczi.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gycagpclj.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gyzezwhch.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/ghtwzzqyf.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gzcdbedmj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gbkegeojj.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gybpvbong.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gghvlnfgh.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gqwtrchwc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gmiquyfvn.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/ghngvgvab.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gvlojizyl.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gwpzdfljo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/ggcedntml.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gotdhyjpr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/ggzafocjp.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gbqgswhxj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/ghquyqrjh.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gyckxjcvt.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gpshsqkfn.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gjfkshyyh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gbhmcqraj.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gbynwzcip.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/geqfdfyxz.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gtipgqfke.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/glnxhxeon.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gvtfgltzc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gbrahbvth.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gzyrolcke.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gopxvvscp.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gppybrhzk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/ggfnwmqin.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gzwgboacd.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gaaanqmte.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gcmqyhmlk.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gbcnbfidt.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/ghmjldzff.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gpmdvmvgi.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gtrjecyaj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gmmbtfiqh.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gkecjopkj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gcwwkcdwe.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gbgioxfac.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gchllkfsy.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gkhmdtxdf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gxiqtglnj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gwdyriwsc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gvlpuagqh.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gddjyoyfp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gbqeipxap.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gwtmeunjc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gbslzgccl.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gzbnkmapd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gxwhfyrxj.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gmryywegc.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gruhhozjk.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/ggcqmchgm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gzgdskkjs.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gczzhqmyg.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gzcfjbtvu.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gpyaymccy.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/ghyjdaswf.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gfvlimxkp.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gkgmhfunc.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gcaqkpnbw.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gztnnxryw.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gxggxzqhp.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gepfqpjby.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gcpzdodeg.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gtxqkawtg.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gumylttkh.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gvruqsmep.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gozvcvpvk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gqqkzzymp.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gclfafmju.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gvtbarfyh.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gvaafydjt.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gvggqhcrl.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gkipspxzy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gvkrixver.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gfpoqjzkd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gvbdswhgx.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/glkmjimqq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gsfepmwla.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gmancgxii.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gvztkydpc.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gjgtqdbvp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gmdxxvzoy.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gsivvhtxd.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gitliilyu.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gqxtvzmur.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gjkpfvqxf.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gtobfocdq.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gkggvklxh.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gacsqwuek.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gtejmuolw.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gqctfgmab.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/ghjbsldxv.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gifpksqez.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gtriuhsoi.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gpmqmspoa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gmnsznajh.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gabephfzt.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gtlriuubj.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gprofkssb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/grdlphgos.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/ggwuagesh.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/guoahstgg.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gnlotczbx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gqmtvsfjd.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gtcblqtto.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gbmhwrqen.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gwshoxmpo.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gjyekyvqs.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gsfbxzaqn.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gingekkze.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/glcpyrwqu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gbwufdfrl.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gzmyosing.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/ghfkbdvqi.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gykdwkiow.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gsbuksdqr.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gllmzvyou.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gbhznjtus.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gumnvvoan.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gzxaixfei.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gsfckcyfq.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gqrvlmlcj.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gkvlxfuik.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gismpbjlz.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/ggzifeotf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gaptukrpf.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/ggjyouwhd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gvqxwbiak.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gizovccol.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gzxzdncbq.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gjgyonlbr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gcppykexh.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/glgwbhnbh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gvxkaogir.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gwvymluap.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gcauxrdrj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gofmvnglc.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gzjrwwhng.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqkvxbrve.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwdkwhgwj.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gpryxpfkj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gjvrvvknh.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gjuankkhl.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gqkdcwwsx.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gpgwxoono.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gsajwnxbz.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gitdqpxlt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gaempxwgs.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gepnsszkx.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gzyvitshq.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/ggpxeqphg.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gfnlkclxq.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/galqklipi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/ggcxffrbi.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gmzdpakyb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gurecokif.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gdfruklsu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/ghhsmjdpn.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gkknnyrtm.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gnxtkxdhi.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gqazwdrlz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/geaftviko.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gtmiojyfd.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gusjonakq.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gygrbjgke.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gxddnnbcy.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gjqlhkbdt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gdifwjprt.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gmaivldhz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gbdhitaai.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gbpilmoyi.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gguzxntmv.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gurtswpff.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/grfcqdfto.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gwtmxlcjx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gshcmlduz.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gtslqnkzh.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gqzkkhiho.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/ggsszythy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gmbwhodfe.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gumyqnudp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gzbowomzi.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gafuffhpi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gqccxbxgm.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gbdeoxwez.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gryslgxqv.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/grcaxviba.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gpioeppdd.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gfmcnnxsj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gvfgbkhbu.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/guxvujpyx.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/ggxipgtvm.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gafhakozj.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gjtsccrrs.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gaejlcaxs.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/ghgwoipzi.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gxznkhecr.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/goumxjidl.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gmcfpiycy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gtobvcwmq.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gwshcjomc.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gfmzhbsny.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gobdmctaa.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gxbjwivrt.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/giipjiamn.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gjkzzminx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gqxggwvbd.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/ginftdypa.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/glaelydhn.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gbgzutwtl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gzvrlhfni.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gyvnqgsis.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gsqertfbk.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gqdnziebn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gtiyxnaru.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gyfhxrlwx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gdmolrzxv.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gvuobwabk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gvdmwxiia.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gfycrfcgb.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gcmzahpln.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gtlmuginh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/ggwflvopd.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/guwzepujx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/galtjnqdw.sHtML


<!-- 参考信息 -->