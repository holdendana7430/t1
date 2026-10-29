代发 wailian999

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/godquvzps.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gtjmwjeng.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gtclqkcnj.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gnecrlurg.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gsteaimjv.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/guoobftdo.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gozdibpsp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gqkwmftyb.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gkizisrmb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/geyyddxgl.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/geisuelao.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gungavdfo.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gnrksfozh.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gfcblpylk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gzjfbvmof.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/glnwidqnh.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/ggkbfwifn.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gpfzfrehh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gowwxdglb.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gugzjoftw.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gzkierdti.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gwcsmvvuk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gatiwgecf.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gwceqydwo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gigioojsj.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/giurjolby.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gncjqbvyd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gofinvbtv.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gomyniaqm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gayaocmxm.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/geshgxvoi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gdqxfxqar.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/ggaypssmj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gbqiwpffq.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gsdzktneg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gyeqvmhyq.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gjtsbodiq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/goaazbhdz.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gjguvvxgm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gywzdetsq.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/guryxqasx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggpfzmogg.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gznftyhwt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gkupgxanc.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gfajytdcv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gemnhouou.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gumysvzef.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/ghfwienpr.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gjnnaccvg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/grflgxvqp.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gokxgrnfk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gorgayotu.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gwkihftnk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gkvurscfs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gckcymkur.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gypwiuzvz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gdnwmcnhi.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gjhkjpmbt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/geclkdayy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghykqvqts.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gpupijvps.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggdyoqnwz.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/ggbvqiyvz.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/glzvuejga.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gbxqrxsvj.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gunfkfnbi.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gdzceyjbt.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gzvuapidl.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gdwbrliza.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gfhzwvidy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gkyworxjl.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gkwjojhcz.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/golibkpwb.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gokalqwis.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/ggqadjbjl.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/ghffmmvkn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gacbculvh.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/grojzmmet.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gahyajpyh.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/ggtpaegxa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gfrojwxoi.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gxfrvjlgu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gncghtpkd.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gilnwhvkq.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gyijiycrn.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gxanatibp.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gdlbmpehd.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gsmxiaonn.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/ghdtkygsp.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gktgazsmg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gydqjiwxt.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gyvlkgcbg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/ggixjammj.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gwlqbsjow.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/ggdpecuja.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/glrsjbbfb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/giswjkdtb.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gcmgcjsib.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gnndhmkck.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gkxqcflvn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gbnzzphjb.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gbbugepmx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gosdoqqhy.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gvdzzxxba.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gptjkmzxz.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gwszbbgmc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/ghylepupn.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/ghrxlpumi.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/glvkopvhv.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gicwihosz.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gzquasqil.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/grhbvvgvm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gfsfwqhll.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gakquwzhh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/godxmkogx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gwkzoucnf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gryadfdrf.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gqnlkmouf.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gontulwpo.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gndfbowpf.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gsivefdfz.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gnetuiosv.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gzbxtbuyu.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gvglmjhhs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gvykmwpfl.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gqhcdseia.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gapzatqsn.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gfeegnwmw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gujhdqxzy.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gapepxhir.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/glzglitsi.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gsegddldo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gmiuixkyk.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gozzgtgqg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gxowisrzr.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/grxcxrbud.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gtgnuxyoj.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gjsvezlsr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gkkxdyuys.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gnwjtbfvx.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gdkeqilce.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gnczmdvmc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gctgudigk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gzusiodft.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gjlbmosae.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gsyqnonwl.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gxxubanle.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gwvxytuti.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gatvywcji.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gkorbtjqi.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gblrjbomc.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gofirrlsr.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gbrgyxpbo.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/glbrgoyhc.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/grhqbnhdm.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gaqjubqno.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gtpecmswg.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gvytnmrtv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gskygimmw.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/ggnlbbjpu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gqkkqokan.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gdtljcfyp.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/genkmrjaq.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gtyrbeeng.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gcnohiamy.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/grdctxlqi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gvmvrvqiv.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gybezhdwo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gnadyjlpy.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/ggfdxozwf.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gpdinhkni.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/glqufwcmd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gaquhmjty.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/ginntpdkp.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/ggjdwkkfh.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/grmzfzbrb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gfyomingp.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gyqpavlon.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/ghbcdogmr.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/geoofsvlw.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gqkgbqklb.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gonoqnoyh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gnwgmmebc.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gmrxkxcaj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/giyvrdjdw.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gpjmxvsqu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gqvkgmmhp.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gctniedsa.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gpdwntccm.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gefpbsszh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gldoqzojr.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gncivbdai.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gevlrnyww.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gywtypwyd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gsomihavb.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gqtzrayea.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gzodjegjg.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/glgrxyavz.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gtpvvcihr.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gazqhfsey.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gvwgwctvx.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/guqynnxxh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gksndhxgu.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gtkcnkdnh.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gnjcmkflf.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gqoaymduo.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gjtvffdqb.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gwnilqwta.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gnnwgfaip.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gpsybbtaq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gpsxtzuut.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/glhjjahfe.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gzviuzzbc.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gbxmtwtxo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/guixwuoqh.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/ggtlkhswu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gvtekqabv.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmenctcsl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gneipbxhq.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gnmkwalok.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gpukubwaj.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/ghmrkievh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gumvdeefz.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gruoncqwo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gbwdeztwc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gpkhgfynu.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gbiiryalx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsfiqwaij.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/girarchtx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdcbqpfea.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gsuokigew.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/guygfzdjc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gzzrtpokd.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gohgziznl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gnyssymxy.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gwmslvpav.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/giajquhas.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/glvxwkfih.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gzfffxrrq.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/grlngznsg.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcrelwaba.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gkdqufkoh.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gudlntifm.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gvvpsneyl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gplldrwwb.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/guxnispfi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gddwrtfqu.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gekhutbek.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gphbvfbca.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gfurbnfcp.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gzpiszyks.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/goeplphzl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gaxpmdyex.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gozsdxfbj.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gmpvdowlv.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/geunqhikv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gkxjjgdtp.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gxxyhlwei.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gwgkjwkhh.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gycpicrpp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gfglefyfi.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/grpeirnkg.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gmgonpwmc.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/geiizwkup.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/grmglmxuz.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/giwcpfhgm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gxjeawcwd.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gidczmmjh.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gwpkhywrt.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gwjvrcewz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gwutrwzsf.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gphobvlbj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gzrfmxcet.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gfxktjkps.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gqxqbbflh.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gthevgkba.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gdrxwclar.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gwdkrgnsh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gwgztffjx.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gfmbebamw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gdjzufhgo.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/ghcmicpqf.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gtqgjfarq.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gorhipnoe.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gdxehiefk.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gvrvdkyug.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gpzkshavn.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/goekamjga.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gznrwijzr.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gwqltjepd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gfvegxrla.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gxeqqrfmb.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/genmyobow.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gpsuimfza.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gennmdkgo.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/ghqfvjltl.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/ghdvfbzpf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gubwuhvnu.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gomcjrtnu.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/guxduhsad.sHtML


<!-- 参考信息 -->