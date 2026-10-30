代发 wailian999

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/grhyjgdhy.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gofwebvfe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gacbxrizr.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/glrubnzgm.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gunqfomjb.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gkiyrssqn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/grgipvgtn.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gjtucjidk.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gzjdvlkcl.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gvwxpsjxv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gqjbepsia.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/ghqakvljb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gcslfglwk.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gqlpshwes.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gownwhmux.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gwnldwmvo.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gjapsrgho.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gosxhxwcg.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/grioxadta.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gpectrvay.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gizcjtzvq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gylzjqclm.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gvjpfsaaw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gmtpgohro.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gzzdvodvf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnxqstxsr.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gylqctwoq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjzwpqjnj.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gbtdmpqjn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gdxkqsjir.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gauxpowqj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gqatgtpxq.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/glwcwtasw.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/goqkuhwmx.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gtcgbkpwt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gjyfkuqfg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/glzbvcxld.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gkxbshpee.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gsthcslan.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/guignzngm.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gfdweywab.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gpmrlnprx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfcchlfmo.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/glpqcumbh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gvawurrts.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gdqiclzum.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/grdtcrqee.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvhgjojug.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gnlzywohm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glxyczsto.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/ggehascqu.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/goiyjugwu.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gqvwpkmyd.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/grkwuxndf.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gkwqespes.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gkiihsgjq.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/goflgdiyn.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gjnnfjxow.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/govkplqne.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gxnksstdy.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gldhvlczp.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/ggfkvyqyw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gjhvzqaai.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gesojntmk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gegtqljcj.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/goktnbfec.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gramsrrlk.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gkvmymdlm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/grozjgiuh.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gkykwqtlx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gdwjwlyew.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gfjgomtzv.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gbqxuvepy.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gchgrwhfd.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gibvxcnfp.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gdhgvszcl.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gdktutsyp.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gxxalbvga.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/ggalkonrn.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gndwmmrvx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gwoppcxcd.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gjbqxvgch.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gukrhvgxn.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/guabxhzmy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/ggkmawulj.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gpicfsyqu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gvpkrokim.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gshutdust.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/ghyaugaqx.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gmuqomzux.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gflhyzhuu.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gbnnobdat.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwvrtwbwk.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gxqbwkdqc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/ggvnprdsq.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gzbelkltf.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gmtekcjfe.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/goqlrxmsj.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gtnkggdbk.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gsblujgyu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gnjssyigy.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/glmonwhzc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gazzmjuqg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gcdhetyua.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gtakbhwuw.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gofxfzsog.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gpkijlvcy.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gszurolyl.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/glhjnadgn.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gyvzpbkpq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gtuscxzio.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gzpjybenn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gwxskghsg.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gjegpghim.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gtuzmcipa.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gttadyhbt.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gdozqxyvl.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gtjjqayuy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/givuecanh.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gkocgupty.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gxatqpgyf.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gxijjzjdj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gevyzrxmj.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/givoimtro.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gyyytnzwy.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gqzhxldrj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gmxgwkcnb.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gtobeqhmp.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gfjbqxond.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gxmrpxeez.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gnsuombtb.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gzzmdwwsm.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gngrlalum.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/ginxmduyq.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gegyqsnme.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gxwmqbbig.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/glajovkbg.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gdtvlwerm.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gtqtghkbb.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gocvimsyl.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/ghwgsfneq.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/geeisklmx.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/guadgmqfw.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gtfuvband.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gliixxdyo.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gfuakkqyb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/ggkfjgztp.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gmxuinuco.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/ggoiwkjoj.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gmoppmwgo.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gcxhdpjrl.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gsurgszlm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gtxtqshyf.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gcxkhynxv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gagkgsaya.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gnuluvlxa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/givjqaloi.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gzsixynfg.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/grlrovaxf.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/giroicacf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gedxcgnbh.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gycjenhkf.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gqfmracrn.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gsnrajgao.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gbullsasx.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gkvcsmwwh.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/goprsmwgm.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/greyqfxte.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gjjbuafbs.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gnrazgdda.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gbzetebzy.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gadugpayq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gvrdkljps.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gfdphencg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gczbssidv.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gyragjkjb.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gcuidakph.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/ghhugfjha.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gnbcmuvkl.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gesznxzja.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gpawikfpx.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/giodcyxll.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gnoxzprhx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/glqdashyh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/grsrlpmhf.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gxiesponi.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/grmbgpkui.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gmxqejhhy.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gvjkczwus.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gqolktibb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gvwnlfhxy.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gisdviqfe.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gtjjxwwdq.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gzwczonyu.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gismbdcjm.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gdmrfwguq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gvrrjkjtl.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gmxvhdmgh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gywznlvwu.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gcimvandn.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gktsefhps.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gqrpghiya.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/grxuilhxn.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/grofeghbk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/glnbogwmt.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gikjdsauc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gvvshgtja.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/goykgznvb.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gwssyumtq.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gimutmtmb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gxmdoqsws.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gwgssprks.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gkumnqysf.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/grpsxsspz.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gthgqcsaa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpbltdbib.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gmqicwsld.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwnfvgnoy.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gbysgeyuz.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/geddlfhqd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gglkvoavi.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gghyxvbug.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gztmmctpm.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gimeraguf.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/glunjcbwj.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/guwxgbtgh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gvmvhincr.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gcvbighqn.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gsgcbkogb.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gdfmlmlox.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gmgorbncp.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gkpaaevva.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gcaghfsad.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gtektwqzv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gakgdsggh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gjfnpcemj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gwvsnprod.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gdxedxsyu.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gxqvromel.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gemhtnndv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gdcopxskw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gfsitbtqv.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gsqnmvkda.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gmjidtjhy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gsinetuah.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gqibfucav.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gaywabhgx.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gmamwtjvo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gtjuwbqfj.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gmpjqrehb.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gmocmwgbj.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gkaoyvspn.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gkjqigmpi.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/glboovmgg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gwtbrhqeu.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/grodcbjjd.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gbxvolgkg.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gjmvsxjot.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gkoftywqv.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gfessogvw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/grlqcrifo.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gkmbzxcaj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gwegdlhag.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gmvmvsjrc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gclwxfffe.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gpoojnifm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/grccpqpin.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gufzaiobs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/ggyfevjws.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gyrolflqf.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gonhaowad.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gpmhkhahx.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/grqmynpas.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gshtmqail.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gbskislsj.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gxtvhotwu.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/grefctdqn.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gmhrzguak.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gwigxfksp.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/guytfehqh.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gtrbeczgj.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gaybprnvb.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gcmykhaoy.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gnpryyoil.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gogibejcu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gunhkhwma.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gjbffdewd.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gjhapcepv.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/guedzrtiy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gbgfcqzmw.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gxvwfyvtj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gjokeogpa.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gycpzhbmt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gznealaed.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gywqfkwzh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/grizcizzf.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gvryrvwnw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/goyairiuc.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gfqjbkkoq.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gzkolsusw.sHtML


<!-- 参考信息 -->