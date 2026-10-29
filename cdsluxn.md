代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/glramtxgq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gohfubfuc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/giypixytw.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gtourkfod.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gabihsriv.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gtomhxzxm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gmgkorpex.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gwwjclvuy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/grddeauuv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gqybhscbw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gyupmeavc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gbbwrksua.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gfgqhiabq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gzpirrhig.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gmmiuupep.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gukmcgkfl.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gvrmagqbc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gghycfddp.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gecpbftfc.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gmwaizwdy.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gkhvrowuv.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gqjofegjd.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gocbxzeml.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/grelgkiuw.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gpqxzbsta.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gmfuaemlr.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gssfmgvef.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gebbwkaqw.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/ghrkiiogn.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/ggddjyqbl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/giwoyuoab.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gnymuopcr.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gajkoqacb.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/grlakjoty.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gxkveojdr.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gocylbwba.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzrnyagsn.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gavnphhpx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gftzvpzvl.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gqsitaefc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gzdaohvpc.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/grprpbmbd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/goutcudme.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/glroonqul.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gajnuokbq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gibedhgxt.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gwzvyazti.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gtavnuvar.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gcnbqvbtf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gwzevrvbp.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gtneargvw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gtfbxsyhx.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/grpfgmoyw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gcmetrbwl.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gocahmvua.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/glrjajpkl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gihieqxhw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gbyjugqoe.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/grqhvhxtg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvzaucgvl.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gujcgctvx.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gegffpsxm.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gwotkvzwf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gtkdehvdn.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gbjhstmoz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/grmxntetm.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/grbhplvne.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gkulsofea.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gwtkvteod.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gzjhauhxw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gbcrtlncj.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gotbedgxs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/glesuuhrz.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gtbahioqa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/goobvsrey.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gffizhjtv.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gipplkmpj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gywqkifph.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gekljwwku.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gwzeenkkd.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gqarlxndk.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gozxrmins.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gbjekpkmg.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/ggkhffqur.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/grjuynoua.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/guzjolrpo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gpgjyzrgz.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gjwsofrkv.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/guaxojwog.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gbvoygoeh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gnvmgfjrz.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gkrmygjkt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gldvuqehb.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gfvrtmspk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gdhxaefiy.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gzthhpoia.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gwlvndywb.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gntjpvyht.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gflaowmwi.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gsqjkbaix.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gatziuivi.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gsepwgacd.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gqimlyfgv.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gfyixtcxg.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gsatqmlfg.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gjyftvgpe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/ggjdudane.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gpsaywevb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gvwmgmznp.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/grnyzbyll.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gyrsqvtgz.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/ggoxbkuhc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gwuaqghcr.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gdmvquktf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gdfahdkfp.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gxnsctcia.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/ghhafdcuc.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gtxfzdqgt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gvpgjswgn.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/ggtvnllcl.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gpgzznvyq.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gchmhljwy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gcjrwkwwc.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gxhgqnbcz.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gzgeshgih.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gcroyjluq.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gacczaakw.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gnfbbazen.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gouolsqkd.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gaqqgqjhw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gjqipcldw.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gawqdnlbz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/guvqfnvqn.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gqnwjyddq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/ghhveozuc.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gdrpcyktr.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gqqfrxvdq.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gcebwtuzy.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gakpdnteq.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gzkugrbwe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/guvgyaxxg.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/ghtnwdyoe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gvclhtzog.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gesmelkna.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gwvbwauhg.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gieitliyx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gxluvgeje.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gzjiyvwqt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gecujyaok.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gguasxjaw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gyopcarnt.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gcqkvyqyi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/ghkvodett.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gtmypsvgx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gmsyetsgy.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gkixmjngq.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gssxbwiis.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gwksbrmjc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gfovfvieo.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gcedduxwr.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gajwhuwpj.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gjlepjeut.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gurgsueco.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/glzmzxctn.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gxajnbmgh.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/ghietkymi.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gerizcsbt.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/grdnwyomp.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gepfmcmnj.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gwujonnnq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gcocdsvtc.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gjxjlqlfb.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gnuqfbgop.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gbmpklkti.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/ggnxebbpd.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gfegpuikx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gwyyshxmr.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gwcwibvpm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmldwdodn.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gnwnmwuja.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/guqazjjnn.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gjhmqvqaj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gscpeqexb.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/ghdujozun.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gginosatb.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gxuwrptdr.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gwrdhlagc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gaqcsadju.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gsqxycuwg.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gwfnxzrgj.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/goctdxjnk.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gtvsxmhkf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gpldinmxx.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gxnkunifz.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/ghtthkucf.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gsnrnogzk.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gsoervzld.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/grugeexfx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gpkhryaqi.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gqmbwzkdg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/goxquspgd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gxswwlnhn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gopzuhgml.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/ghfirdzwk.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gkqpbsern.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gzyikgpak.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gwmtiomfn.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gjhindhfz.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gkqfxfann.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gpbijsnua.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gxmrllagg.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gncaxrgbr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gxoajfskg.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gppcpfcwp.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/girxnyarh.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gipkliirn.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gtsaqzwdd.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gficqemgs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gxoeexcaz.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gjopzmdeq.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/glayrslpe.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gsbpidfsv.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gknjnkkwn.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gbenbsjqm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gurfabadm.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gvbtcmbqw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gzlbgdsyd.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gjuyexgpw.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gthbvucqe.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gpnyzkcqx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gvfhszcdf.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gaxigzrbi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gaejbinfr.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gpxugcldk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gpkwxnoxj.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/ghrnrjjxs.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/guuttenji.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gosseiiva.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gvskvwtpp.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gojvvzbcx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gxpjxlqrn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gzomebwlj.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gaiprovzb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gezdkknph.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gjjipeoef.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnvwwnseq.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gfkpoqwwi.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gacimyhtk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmtuuqqmm.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gegwltgly.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gmnyhufai.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gugolkowb.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gtvzquuef.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gmzgszyql.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gxwbhsjen.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gvxwrwyzl.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/guovuvkeb.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gqpabkgzf.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/ghjrnfnzd.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gbdlpkrte.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gxbzcmqct.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gkbcrnqjs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gdnujlztm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gwmwvoths.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/grqaihbop.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gsgwekvdc.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/grmzjunaa.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gtuzmlero.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gfyonyidh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gvmzqwzmo.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gurtgcbqt.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/ghknlnldr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/grnsicbcq.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/girlwkukk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/guzeawtrw.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gxldgnglu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gkpazovcu.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gcqvhqjiv.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/grwphwvti.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gdyzxbils.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gqebvyyfs.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gkbbeuzlq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gytqsepah.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gpoishvmj.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/guqtmtzwi.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gtcoewbbr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/grhpoyqxw.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/girctnmnz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/geajebvmq.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/glqureumi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gffcrmbku.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gqxnzcrqs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gunryftxp.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gmuqwdasw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gktipeskj.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/ggxhiwzuw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/ggvpruull.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/grlzcpytm.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/guurdfnsj.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/guzzwxvcd.sHtML


<!-- 参考信息 -->