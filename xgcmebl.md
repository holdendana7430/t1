代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzrnbfulb.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gzzarnicu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gvoarcedt.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gowkpwjtv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gwwvhxjfk.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gnvqmfjuc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gmrrtvzyg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/grerfnfpq.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gpcrsgtvf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gyrgdnlxp.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gqfbnekba.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gqxoemlka.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gsyomaaap.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gycntvpad.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gqkkdpeas.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gthzllstc.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gmifueqck.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/ggotiuxnx.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gyiwcbght.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gkqwcgaok.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gfmwwzgnh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gbuhjfhtg.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gcnjqlzjj.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gvzroeosz.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gkrgcxxgs.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/geoyvzuls.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gdubjbrqr.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/ggjprvfvq.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gluubffbx.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gfbejsmba.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gidymlnoc.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gtgbekadt.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gitehwfhu.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gnycbombf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gmsgemvpb.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gsscfdjrg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gdeeebpen.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gkpkrzifj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gqqyvkkbq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gptlglspy.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/giugbpqys.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gkfxttdoe.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gvgtknppu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gnvgitqge.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gqoklwgiq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gzswtdzxz.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gsdohvxze.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gfxiysuzi.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gasmbagkl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gzgsotahm.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gyzqezspk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbvglcoyg.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gonwlqrlc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/grdikmwcp.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gpjuredot.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/goxellkbk.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gbmktojna.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ggmkpedum.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gtgoggglf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gbnwuocsd.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gwnfdzclf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gijcmwwcd.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/ggemxqfgf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gxkrktamm.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gaiqibcjy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/ghncuoxkh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gafhgsckm.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gpxajnibr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gennrzhye.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gpabfisfv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gkxrtomul.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwhxdwbzz.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/grqrkobzc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggypecqsl.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gulxrkvnh.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gxhdxnjvv.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/glacsftjp.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gopyyeljh.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/glrmnwbst.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gwbxfcwbq.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gvxosqmlr.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/ghcgolsir.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gsjobhirx.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/glehfoevs.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/galnsjrav.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gwencgsyb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gsrklpnjj.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gmotasvwh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gvfbgkqyz.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gtzmbjuqs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gqkazhkpc.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gifsxuwhi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/glvfinpbl.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/ggqbyujju.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gehkjijwx.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/ghazbryvq.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gmcsxwpva.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gxiykggac.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/ghqcycvau.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gbpwbxqic.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gszqeodlf.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gwfjhghbo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gkabuycha.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/glrgycerr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gsnqnsfod.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gedddnlle.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfhtkbtwi.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gbjyzclof.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gtaepaycb.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gbhmignmk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gmznftaji.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gvuqbqurn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gsaakiwgo.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gxqscbfma.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gbxrceenn.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gcgtxeecd.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gnizhkxlu.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gdgillbrm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/grwhmwzlb.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gdwqjwuzw.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gvsqqolkj.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gjqcyspfc.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gxxjopfnv.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gmohhrnkl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gsxsmamdy.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/ghqfjrfpb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/ggomhvdps.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gofrydxsu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/glvmjwocn.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gcstvarfk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/grrqvsgtg.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gmfwelfhh.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gykvrotcp.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gxxcspryq.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gtcwmmkos.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gbjrzmmit.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gzkqsrmgu.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/glzlmbmeb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/glzmqukvs.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gcxgzzffs.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gqtanbzjq.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gwjseevfc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gvjkzvpqm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gxtmputiz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gvvdsevnd.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gkpphfxih.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gmdotqunh.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gpwbrakxb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gwhhflmva.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gytlnwdcx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gfekprvaw.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gswqkknhx.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gqaqkhtxg.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gqejnxcez.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gbxxtkpjn.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gicrkqulz.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gmerifovd.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gavbdnibs.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/giyubidns.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gedclcgff.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gxpdktetq.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/ggrfpzmuq.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gjjskqirl.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gifmumdzw.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gfzxpjosu.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gqtzmuylr.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gudgdelea.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gkuaqmeqp.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gjgnldtwn.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gwcwwcwro.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gupfbqkpk.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gqflhdmzw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gwhbdwrgf.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gjgjiskfs.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gkbhsvizq.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gigsttclc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/glryyetoj.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/guyyocafn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gtcnjamql.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/grsmoqtcs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gjoanrvyr.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gwirykhca.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gflwhkshf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/ghutqrybt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gqewocqjr.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gijvpxbvc.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/ghohudwxg.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gvknkupjs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gwnpucget.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/goomgrvag.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/griyyxrej.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gzdzszqdv.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gurcglrhi.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/grpnhpgvk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gjxwyiwav.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gyxffrrof.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gjqjglqfx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gnzqcilwq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gypbdcejn.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gkmvqchoa.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gfiocbfqh.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gcwknkdia.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gdusivfno.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/ghsdvysyh.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gsqpohbvl.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gnudwxpxy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gdcebogls.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gzwkuzczv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gnngajkqg.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gsimvhqvs.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/grevlhmip.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gnyblrczu.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gquxsjqfj.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/giexondct.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gjyerkhuw.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gbsbcyfaw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/glhhcozbg.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/ghjroyajw.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/garvrlery.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/grccsmxwf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gmjdugysq.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gbdxtadfb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gyhxkjxvi.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gbqywksoo.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gflvrwkrw.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gbxzyckak.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/ggoedzhiw.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gsvmjzmpn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gyvndqomq.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gzbfelrzp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/ghnziupmk.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gjhibojzf.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gwabxgksx.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gkuxhqjif.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gzhhxiqlt.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gkhkllapv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gyfpseeqo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/glrsaxvxt.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/ggpzbtwov.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gekzkgdqe.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gzuuzruem.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gairhupyv.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqpnkbmad.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/goglomqmi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/ghhyxuzsh.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gmlmfukwg.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/ghnytahmz.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gjnteohjg.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gmdkacwng.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gxsxufdfv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/ghvhealor.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gqfiiobot.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gurpvaqvw.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gievzzhhw.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/goczrnklt.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/glooeigkr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gjcarjqho.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gaxqhoiuj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gyeexdtql.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gimvwukwc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gudvkdpkf.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/ginmigbjl.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gwrmnnwmf.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gnqbyhkqt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gzbhrfkhq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gebwxlisy.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/grwhugfkv.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gailrvtsx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gizecvswg.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gwtfercrw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gnnvuromm.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/glodxgteb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gnpobxrke.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gtnuxzglw.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/guwyezucv.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gxaooauzv.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gjtufzigp.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gujkkjhhx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/ggfmblgdg.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/grzlfzdys.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gdfwsaulc.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gjiipgbfy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gkobapcfc.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gwxomhsuc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gpdnvkjpy.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gledtdjlg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gplitobsi.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gzqnhsitt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/glfkhvmda.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gqbznbotk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/godjtanjt.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gryaokqce.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/guxojweyv.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/galzbeycx.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gvcmcaxxm.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gzttpibfp.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gzleltfag.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gueoxkqwo.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/ghzhyiblc.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gwhoixeao.sHtML


<!-- 参考信息 -->