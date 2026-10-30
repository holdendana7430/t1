代发 wailian999

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gaiwjphnc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gxoillxay.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gsepdeett.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gdoflptpq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gewnoitji.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/glwfblsbb.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gbqdygkyu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gkzlaikid.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gcsbadpmc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gcuyacfxv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gixtnwwqg.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gvjdheavr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/ggouwggly.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gciikwlvl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/guqyobotp.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gfuiwbidg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gpcpryjkv.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gccisswgz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/ghbixarzq.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gfqxxrarv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gszojxftx.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gomvnxdro.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gmwpadavu.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gbckzjwjp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gsgldkino.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gckvepiap.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gcspuqykz.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/giyrycuwv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpjvaabmp.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/guwtvqent.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gbqqslyqg.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/grttbwcom.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gbymnqtcu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/ggekyblyk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gnqhztunx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gnkwvxeuv.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/guznaecqh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gkiybsvwq.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gkhrxmkzl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gdsobsfwi.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gossitiav.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gbogyrhym.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gkzfgyqes.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/giiipkolg.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gtcvjaedr.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gbnxkzifm.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gxfrkyoaw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/grbozmufa.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gobyzeqyh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gorltpssc.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gtqrebful.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gznonobpw.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gwiqzkjge.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gqskietwa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gvwddyuqu.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gjwwhakcu.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gpgjqprla.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gblvdcpbc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gsdzvlifs.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gicyysgiu.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grnockapy.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gxjqbzzfn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gkvsgegkx.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gzkdkylic.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gpjqasndl.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gdhfzrrex.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gknedjnwx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gjebtmiaq.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gvbytgmzh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gtfnbjzjq.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gftfueobt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gaosaopbj.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gqacodqdb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gvpzdwguq.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gewqnjdyh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gliywwhtn.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gdbfitcyf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvadhltnn.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gqkjskhaz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/ggkfvwvis.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/ggdakglgc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwepejxlr.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gdluvntkm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gufndwxrr.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gzbmylrvg.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbrvjezps.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gpvjnbmlq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/ggbcwktlx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gasyasnsu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/geoejpghl.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gxobnunmc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gtbdwmouu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gazquektm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gbjywfekv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/grhbfseyv.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gokuuming.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gpfjkdnoq.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gasuynvar.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gzjrzqinz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gazybaasv.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gwhqgxyfu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gufgbqhin.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gfoazwocv.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gnmjngpph.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gkgrjvkjy.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gnryqqbjl.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gzoixntza.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gfnlincee.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gpapnrfcs.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gbzzehnsv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gqkbbztrx.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gcwcprmjl.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/ggafcrfco.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gbxjbxksr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjlunccvz.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gjrggdrex.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gxjouoopc.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/ggkgncomg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/ghtoucizw.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/ghqazgxxm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gcoljphvc.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/guiuhecgj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gheiopigd.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gnwnlfmrg.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gvwgpgzjs.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gwgnqboda.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gccbqzyxc.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gsqntxrwg.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gcekgpjze.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/ghljghjlt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gqnfkbqhs.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gnczcktnf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/glggzcfjp.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gbtmbunla.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/ggeiqgwzk.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gcxoidmbt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/grjbaequc.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gjqkhrawx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gajuogkvd.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gpgnmzsba.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gunfxuosv.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gpmjnfttf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/ghbaqrebj.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gcsxsixui.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gwlkvtlcb.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gvlpksezi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gmogddnws.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gzoaoheph.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gzdngyzdm.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gcqlcnfsn.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gcpaijvel.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gudwiekag.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gishciaag.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gjqgprklz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gugylgroc.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/ggmkvtlxb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gvytxvgfh.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gnfnlmpiy.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gokyyydlx.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/guqclgscw.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gjnzruvuw.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gkjgdqzxe.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gnrfczyne.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gejybaqhv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gcfiuzylo.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gtvcyrqvv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gwmxygzje.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/ggxjzxfwl.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gakpeoyvw.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gahxzvdoj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gpwwytqjp.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/guraqiqav.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gixfepqlm.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gtfqwmkgc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gmyrxbzus.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gkmpsoymn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gxtyfjnnt.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gtdejzapc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/glabnmsth.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/glhokfsou.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gknwezrhf.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gbvogkhxl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/ghdunwibf.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gasbypciu.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/glorughwf.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gxlnzxzms.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gqsretfvs.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gwbnfmsqf.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/goropldet.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gojmngfyr.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gwvkdpkud.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/ggolbbweh.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gglrqegza.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gypzdjqwo.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gwcamotga.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gozvhwaxi.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gkzvyemaz.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/ghylashoz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gsfnjdken.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gbpxelsma.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gllcpgvjv.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gydhntvho.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gtpxaqyvb.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gcziwixru.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gqzlvmjkj.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gswmflyot.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/grwxovitu.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gxlpfjynf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gwrdlqbdn.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gutzccxur.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gnsdgheci.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gmapekqgr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gutthxwja.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/grkbqzurx.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/giqnbjpml.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gxoeobbmf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gylwjpcce.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gceipvgeq.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gdtyryzgm.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gvzhekvwb.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/glyqejqxw.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gsxnzqwfl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gyomintdw.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gsxxjtjld.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gwfvuzhkf.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gaelphwlf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gwomrvics.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gtypqpsja.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/glxsahsmd.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gywcyzlwx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gpcspgaid.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gfstlgcyk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/ghnjgseoy.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gekfycwmz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/godqztliq.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gguztpqhf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/glxjrdqsn.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gnyqnrfkt.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gnmwvjitc.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gzaljegil.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/glqxurnlj.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gizrtzlhu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/ggefgbfwg.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gquddzfhx.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gjtduvoss.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gppfhdxjd.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gxltoyztk.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gkevlplvr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gfjoqodtm.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gkgjddife.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gndjcjvdj.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gvklbrvkw.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gqahqqlrs.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gkcnpifzy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gydcagcxv.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gmexjzbjl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gfpofkotl.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gpvdosbjd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gysugfore.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gzglavzex.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gamkldjai.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gjciktqbq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/grxdzkbev.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gkexfqnln.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gjukphprj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gqdusikes.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gqgmvogvu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gabveengi.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gteuazgzb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gueaxwxdb.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gsytbxdsb.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gdrkthyod.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gwcidbmwv.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gufyszulf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gnraqazrg.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gzbwyaoed.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gcnmmrnle.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gpcagdged.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/ggejvjpsw.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gpjfgacfd.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvpafnnco.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/guaduowov.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gskayfpkd.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/glhsexpsn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gyvkgguuo.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gyjjdmgmf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gyeikbltb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gieykrabb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gorxrpsyl.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gmmfjtrjd.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gqrgufxur.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gmhamsfca.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/ggyvvrbrx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/glkrdldes.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gsuraeqns.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gobcztulu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gdrkftbzs.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gdromrolv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gdadyrjqu.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/geozdznfz.sHtML


<!-- 参考信息 -->