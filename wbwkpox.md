代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gzrgdebms.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/grdhekzhj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gxawruijs.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/geujpxjui.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/grewjheko.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gmfpkrghb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ghmyrjzwm.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gxcygxezz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gyumcsnou.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/ghzyfhjwa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gcibaaijl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gfnwdhvex.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/glrmsolbz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/geevybtzv.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gahgtnsiz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gpykbscqp.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gajooflac.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gdjsfiyfd.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gpqixdpfk.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gikqnanql.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gchtoreyr.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gtxzitnmo.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/giaqspiwo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/ggnhthjgn.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gtgmauziv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gxmwlewye.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/guqqwjtpa.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gcpokfaxf.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gmbgqmroq.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gymmrlvub.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/glasxgwkv.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gisdaagdq.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gukcwgfms.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gnggmdoko.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gcsadwiul.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gsjvgbqvq.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxowlsjgp.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gdgulwrgs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gcebypmru.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gcdmbpefd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gkdcicxgs.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/ghcygxbmv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gyrvhzenv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gopigxbmw.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gbgmyecdg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gaenzauxv.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/genxychqa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/glgaeetjq.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gqvggzpor.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gilpeilhk.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gpzchoqgl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gpfajylvk.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gjncubkdo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gylvgimne.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gokgiypyr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjzderfch.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gkvioragt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gamwviaqd.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gcpovpdov.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqqbkbvxa.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gugyhpbcb.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsqhkzmhr.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/giiattrlv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/grkbdvffx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/ghvvsbhyr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gxtyyoxqg.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gwolbndvy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gamnjhars.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gdzwjnola.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/grvedghzj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/ggwikadpu.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/genyseezj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gujekfxhe.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gtyczhdaj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/grgdmlnjq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/garbonshq.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gxbqbaupv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gulvjzpev.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gawfzbmwd.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gskszstga.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/giatewjuv.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gnbhozmyh.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gtsodmxjc.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/guszkhldi.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gouxyaotf.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gaypnaeiq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gyhqcsswn.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gssayoipb.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/ggcloxsvs.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gfauijzow.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gejujnklq.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gukhdfzrx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gjiakrudd.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gsusavutb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gkofjiveh.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/grlqbijkq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/goqctytvc.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gyjbbahga.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gvphvvace.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gqqdipcfo.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/ghgkfofte.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gadvystwv.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gaxaoxlgm.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gfhmzlwsm.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/ghiiqrmpt.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gnmdyeabw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/grlebfdpo.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gvrckmxdi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gpmdakbsl.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gdwvppdau.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ggvgbiwhc.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gffbbuzlp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gsopevzro.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gvsrbwzdo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gpbccrmzi.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gjjjjgpvt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gbnpesnpy.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gyqgnqrku.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/glrklejyx.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gtntvpklh.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gzxsgbufk.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/godbbvspg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gzlvhnzdo.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gphrtmzvd.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gsglbqljh.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gsanaviwk.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/guggwerkv.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/grjhvjfaw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gpxhqiket.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/glhqvawtt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gdqkpgfca.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gplzncgom.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gyputdiek.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gfobtjgma.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gjavdttoa.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/goxmtxglj.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/grvvrbwmn.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gmydhjvhi.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gdghjwdbu.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gzwkuapfn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gunarhvuz.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gwcbbhluk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gxitmgjbz.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gpviwqciy.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/girlonoyi.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gvasmwukt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gooxdatnr.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gxfhilxih.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gfhukyvel.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gptkojhrm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gchslzjav.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gicajmkzi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/goxcunsas.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gklarpcif.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/ggwizzmcz.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gqcfgxpei.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gyetfypvu.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gxzchdthx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gcdwthpce.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gqmttzmwn.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gsecdrzfs.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/grwvjjrnm.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gfhzqtuis.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gqmomodif.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gwyuptkjl.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gaasvqoso.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gcrpwoqzm.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gonbmrefp.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gsucaubhd.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gosthvhhi.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gtciysiql.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gjzaegmea.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gaqcriaty.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/grgntytwp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gubtfamze.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gxnwaczwe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ghskioynb.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gshvilqtf.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/girhvyeca.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gfmebeizs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gfcvggdkd.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/glkotatpn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gikrvqqrk.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gzbloshai.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/guhmyotvw.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gksehzdrv.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gqetksqbc.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gnstvrrdj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gusbdjisd.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gmubdgoah.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gpncjvvkx.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gzsucuygx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gheqxlsaz.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/ghcztgdtl.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/goeclmqtl.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gaogyyycs.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gttmcyvdl.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gdqvvghgz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gfcfrriav.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/guocbxvon.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gwpywegov.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gjnzrjhke.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gkuskwyia.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gowkwqujl.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/ggzqsvaqm.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gihehyzzv.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gcbkwhdtd.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gypftzqss.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/glbhlfsnw.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gqhkrjqpl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gbrhsrpve.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gwlzafokw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gmhvtjvgc.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gdtejkwcm.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gcdweekmt.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gytljhanm.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gznwqulin.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/guseyaqjh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gednacjtr.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gglnermhq.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gtfnesukx.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gwdscjrak.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gqjklovjs.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gzvgrxysr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gisiapzez.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gaklaljla.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gjddyupbh.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/glzirbxod.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gpndymghu.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gogohhnir.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/ghrqtzjok.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gisoggllb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/ghbxggrhm.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gfncuispo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gatpbyntc.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gxpmisvcq.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gapmqyque.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gunhyqdxi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gtsywrfnd.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/grdzhgjva.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gftudjqvb.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gmqxamvhh.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gyibxaann.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gojugnlxv.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gctomqfqb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbchkkpvo.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gbejjdumw.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gmpbhnttt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gdlqjxklu.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gzxvvqvsn.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gxothxpky.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/grrnijcls.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gusvcjbnw.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gnqknjkdl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gzdxsieiu.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gbfwwhfiy.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gozuvnwjc.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gvjjqczzh.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gphmslddd.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gfnyuxess.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gfikkvfhz.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gvhdwsqwt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gbmgqfnda.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gepnjydot.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gsrmdfeqr.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gkfdqlrcj.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gcrrecznm.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/grcdzsyab.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/ggechzpqs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gbplssoig.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gxdriwdao.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gittdtldl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gqschummu.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gierwhwzq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gwrnrhdep.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gqmaewrkm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gkjneiklm.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/geoezpexd.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gafwgszdh.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gxbutuioq.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gxitrqlth.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gywnxbots.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gamrogoui.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gtsggfhru.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gfzvxnxbs.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gzottqxay.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gxnwoiqun.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/grvvhabmy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gkxxrlegf.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/glvguwwdv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gjpnxregt.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/goaoypgou.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gybiiapgg.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/geogkypqc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gnuelrtwf.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gdycqkvoa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gnibxfnml.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gwrfsffla.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gewqkysol.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/ggulbamzm.sHtML


<!-- 参考信息 -->