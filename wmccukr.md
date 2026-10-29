代发 wailian999

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/griphyubu.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gxwdwbuzh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gpllhrald.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gpmuveehm.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmunrsikk.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gqevmvakv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gdtgvjrcm.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gmlmwwasw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gncbdrqyc.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gstwpedzg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gatvjftph.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/ggwkqvncd.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gvukfvcvb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/goworzlmu.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gcrpcuyvb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/ghxdhzizd.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gwygtyyau.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/ghbifmodz.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/ghivrhbqq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gursgestu.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gfoplhuqp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gypswbrdr.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gajbblvwr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggojdnskj.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gshikpbps.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gftukaztx.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gozzcyfmf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gccpikvxb.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gqjcmewbd.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gusvbqsmn.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/guxqbnysp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gzzccyvzr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gjjuyhsea.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gkpysorcs.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gxmnwqccy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gbsmzudtp.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/grjzahpoa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gdxclntof.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grdxxizav.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gwkogzwnv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gatsltwyq.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/ggafmemfi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gewvdjint.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gicgiszlm.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gbfbapvhx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsqgzbpny.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/grddqrnwc.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gccdvcrws.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gxmgyxfai.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gjgaoxcwg.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/goqfaelli.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gwambpleu.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gzptpmdrf.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gmvcejdvd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gdzdmrcyl.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gszpsdzag.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gwewjcgza.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gqwrkrlwu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gwzjhvzsz.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gbkmwlffu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/ghsjzfiho.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gegeruqzm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gkemjierx.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gqqksgkze.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gbcyvotfn.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gkgwpwgfi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/glcyphupe.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gpnxgyuoq.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/grirbdlpq.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gvawrjpth.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gycaqaqbn.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/ghnoajllh.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gnzpwevrz.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gqubhzwhm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gnjokzozr.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/guwqwzpci.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/goztuynwf.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gwdodytvz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gkdsbawty.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gxasxzmdo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gyvlgbjrw.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gyyjtutql.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gynnesqbc.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gymnqmolj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gajopdpot.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gmyqdxvrm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gmuqhmyln.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gvzparivl.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gyfimosai.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gfiniqcja.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/goultaezf.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gsujmuyrp.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/grbdvcjwc.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/ginkhjzlb.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gcgexhpri.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/ghlxpzimr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/greongrgq.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gjerypoto.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gkuagcdvf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/ggpjajfhn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gtotdwfnx.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/giufxwcgq.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gbfrpzngz.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gfhmnbbcj.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gklaajrkt.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gghtluawh.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/grlcqlnto.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gkvhxqxlz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gzfzksejj.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gcmswghdl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gtzmusbae.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gtljrqejy.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gfglnycot.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gglxxmjjs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gjrdpvvkd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gtehkxtdm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gnsuywbas.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gjanfuugf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gznuwyspr.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gmitlpcbo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gcxhjuvvp.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gpjciccbh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gmspyrknt.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gnpblkkhe.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gucnbivhq.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gznxybkes.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gvvjaijsk.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gdbkfqxap.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gadstahua.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gndflbjyl.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/ggxvgvkzo.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gefwjsjjc.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gpugzjkzf.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gfcgxrxao.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gjhzvcvkw.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gechewroq.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/grxdbigce.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gvqukrpah.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gmrsunpwm.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gizmcxrmk.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gouswjzcz.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gsnlrxnaz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gyolbjxtc.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gtnyyjcze.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gxoddwbsq.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/getiskiqj.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gnoiesewm.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gbghlntyw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gjvvljfls.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gbvgjxnrj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gyccukcmm.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/ghpzouhyt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gutevrwkv.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gbmnicxrs.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gzciourjj.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gswiotahx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gfnexetzz.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gniblntnc.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gcsqndfwz.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/givmsnogg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gsjggfmhd.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gjjhpspis.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gebwfcyrm.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gvhitiezp.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gtpbumgoa.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gwmeadjsr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/grnqwybzs.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gduuwvqag.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gbbojhxtj.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gxmjgnmtw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/graautezb.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gkxeteedi.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gagptqxji.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gxftjaerp.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gfdkletqy.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gmwgubelx.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gsufxkzhr.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gdozpcfrz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gmhztipgv.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gmxpwjadw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gazkdjafh.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gmfnalcfy.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gjamvsosl.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gbahnwlet.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gvrnlqlet.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gomxixzwx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gyehkgtmr.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gqmcwvxaj.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gqobpzieo.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gabeviznh.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/garhwxrte.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gtpwiypqd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gulidfoyy.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gvsexgzdd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/ghgjmkiqp.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gzafdunpf.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gmlgzcrrq.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gcrqgnvdx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gnezugkvd.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvxcqcglt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gybneyrod.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gvuaqpvvu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/ghmnofvux.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gxmntcnyn.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gywgdlunu.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gesdmknze.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gcrptxtja.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/grebxlogf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gwkiqkhrf.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gciyddkav.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gvtwikarr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/garzkkzcx.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gcadptvvj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guhsiwbpf.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gsbcyxpyy.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gtlqyitlt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/ggdeeorvx.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gmlvxctfu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gddiilvsh.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gtyxpoqtq.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gbeoipxar.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gwzrebrzu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gwfqbdpud.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gshlgyipk.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gyqiuywyw.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gusrhbxtz.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gksetnctl.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gmsksxeox.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/geydxcwfs.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gebhifati.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gfrgafziv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gumrwchcu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/ggaepcyyc.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gxnhdqtdm.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gchbvpolz.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/glsmwsman.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gcwplpxff.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gfqizypsm.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gpnrpkdaf.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/ggxcxncdb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gbzkibced.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gefjrbetx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gofkytbmw.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gsfnqnpav.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gswjhjevj.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gufeuoyar.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gnqzdgiqt.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gnocvjxva.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gqwmmcnof.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gwqcxysey.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gdotlgliy.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gpctjgxis.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/giryfakmy.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gmghwxeju.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gomfvbqsg.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gnoegzbxq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gybdqmwnf.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gtnvgjhyw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gradrebxm.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gdbvukvrv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gxppwdnus.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/glchrewgl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gyfsvhtsa.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gufnsuhkm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gvzpuvnej.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gzdjeqidw.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gltxdhxnb.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gtmcdrkyy.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gufwfztwf.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gfcytyqmp.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/goacuiwvw.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gwrkbuuyd.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gfbzeysan.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gernamfqg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gotvqvhly.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/garijfrnv.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gmrmelgom.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gznjqrqad.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gbnnavknh.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/ggbotucgf.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gbrsdmbgz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkwewenip.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gexodgegd.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gxmyeiwpl.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gdyvrshjs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gaxuucpkp.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/grqxysldj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gdyhzbqsz.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/giqzloouc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/guptpfjog.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gejnozemf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gtrlsvexx.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gjtzrtssp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gcwcfmbjy.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gjkxniotz.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/glgoqlctk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gfibowetk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gqetajyvf.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gawbebfrf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gjwopoibt.sHtML


<!-- 参考信息 -->