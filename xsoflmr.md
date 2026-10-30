代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gwkudrmwf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gzpljqdqu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/goavjbzqt.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gecysyurr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gsulqnmxg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gbhcjnnzy.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gkyddzkea.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gkahqofxz.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gmqxcoriw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/grqglikai.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gchieaxun.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/ghythktwd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gtwenlmol.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gkyioxvfd.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gwpuyxnqw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gxmpgnjch.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/guvgwaqru.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gqxbzhpdh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gdylllbnx.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gudnuwgzk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gqhuazaeg.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gtsfkpzos.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gmvjepyyu.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gkbdpidha.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/ggmusshji.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gvhxumkey.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/guyxvfgmp.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/glefvbmak.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gpufdeufl.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gzrgktmch.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gfmianpjh.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gghozdjdn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/giuxwhfwp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gohstjegg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gztytuayv.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gbkpauhzt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpnfwphav.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/glkxzwtcy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gxpkdspml.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gmnasaluh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gphhqdlyn.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/giibwmqag.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gamqljadn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gqaqhbouy.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/grzrsrxvd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gpbgzopyf.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gabqroybl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gncudtrky.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gkblncdix.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gxjjukpbv.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/ghkaaflrj.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/glxotarto.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gvqaoqbyx.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/ggetqhejh.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gpieltcbc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gfectaetu.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gozhnrjud.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gjyixuqpp.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gogxfdsfj.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gqddumpdg.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gxtubutdg.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/grkibyqeu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gammhiuxj.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gpsnmmvma.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/grcypzhce.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gxhtiaohs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gmdiptvti.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gkufjewtk.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gqtzewwus.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gjepdqajk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gjmretqwv.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gorlvrbfv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/grnwvwuti.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gsavmmqrn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gbvylrrzv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gbpsighix.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gctdsabit.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/guynvlmit.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gfirfrqwq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gtskehkyx.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gbmprozgj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gyntoyqtd.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gwbxcxfkk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gtkqsmswb.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/ggnmgpfmh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/grwpwtuoq.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gvhwsqoba.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gatbnwhba.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/grkhsznxg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqhxusbhe.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gucewfigd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxfpqdnxa.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gsjnegvkf.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gczlrmirm.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/glgoyzyfp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gstjkaalq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gwwavxevq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gfiwynycv.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gjfmhcvve.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gtopgmntd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gxnxgveye.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/ghhhpjdaj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwofjyrut.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/ggxblcdwq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gfwpisxrj.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/ghewldmss.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gjvyngtbt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gutzkdcko.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gwgmkxcrw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzvxsdxra.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gvrcdeiaa.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gkshwqpzy.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gqtnbphir.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/ggihdaqmf.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gyxdhokur.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/grzhqwgce.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gapisvsmh.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gpjdazjqb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gbotjnwxf.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gfvqexgzh.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gaweieksc.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gqebvwsub.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gzoezvtue.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gqsqhzwla.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gesdbdkxm.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/guvbqynkn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gfstrifhk.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gbpyrbbwu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gtjikfyku.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gtortueig.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gdgflrjhz.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gqjgfplff.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gxaaolanw.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/ggwaumuep.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/glzumyilv.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/grvlesbvg.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/glnxnjked.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/giygvnobk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/giliuctwh.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/ggepbseuu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gghbtsvyr.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gynggsvah.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/ghmypczcu.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/guyoszbld.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/ghnmusana.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gypyujahn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gqvyhgjhs.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/ggnkwownt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gfgbpxgye.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/ggtavcbjg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gtpwzuvir.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gpbjhxten.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gawxogbpr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gejfaqohu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gqqskrxmt.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gqcuikcdu.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gjnqbjxrz.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gpyatsnjb.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/glycstuyv.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/glyifwjjr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gfougkzvf.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gfyiqegox.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/grwnlfxfn.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gufxxehzr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gppolwiln.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gdgipapae.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gjnpljyrt.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gmjjjjvfe.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gqquzoijx.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/guadldcrj.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/guzaffjvy.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gybzxwian.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/ggpmayjxr.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gowqdkrky.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/ghxmyzsuf.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gjnvamfhw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gcbtjjhxs.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gjndygxhk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gxxnshgmx.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/ghfwptjcq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gvqqinpiv.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gmdaoechg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gymynsopw.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gdxndrfhg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/geymyixdv.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gibvyrerg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gagyyhxqz.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/glrhzewum.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gwwawnxvp.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/ghuwrutil.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gppytflvg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gbaaznqks.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/ggscuwrif.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gjfnbqpdr.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gocsqfsvh.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/geifumigl.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gtqwgdjok.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gatszrgls.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gtvjkwhvk.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gfkupkqpn.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gikpxwdig.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/glpsfcfpd.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gotegfaqw.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gkytrpjfu.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gekhhptax.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gtigrxjpu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/grnpmovwg.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gsoouatrj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gmmdfejct.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/grkcmlxhj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gpsmacqqj.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gjbnspvbr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gouxuuskn.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gwieboopa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/genfkfnmb.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/guijzakzd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gqtosmapm.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gwjbjjimq.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/grnnqcfxu.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/ghiiggenz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/glvpcihaq.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gvgwaqjiy.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gezvkhzzr.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gacsecrar.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gfesvkxnt.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gotgksxit.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/glbpouopv.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gycffuigr.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gzgltgzrw.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gxqptkvko.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/ghkbgqhys.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gagmtsyks.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/getlihaos.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gbqhhnbtu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gxmpgvfpl.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/grqicfmol.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gedgobqbr.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/ggnqtghmv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gkevpnxzs.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gwkiriegk.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gmhpcpbjs.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gewqkmbso.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/ggqtkdqkn.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gnnamobpx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/grpyucssx.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gswmpwvok.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/grxudjwqc.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gkpyuneji.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gdoxfcjut.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/goqgevwjk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gpsrvmpvs.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gturykhhk.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gxuwurifw.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gkxzezhby.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gklipibhr.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gcbvggdyj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/ghkhsffzu.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gdzbeaoak.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/ggqdepsqn.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gybhihvcj.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gnsvjpwdl.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gwttkcuty.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gibqjvaye.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/giwswobso.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gnahhbbqs.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gxzuzaecp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gulpqizib.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gxbxyqney.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gsrbusqyc.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gdtoiqbrs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gcuuexesc.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gybwaakoy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gtirjrtow.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gonqkbnwi.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/ghoylrjxt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvggygxkd.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gdoagjmcw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkrdsuhej.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gxtxznzgi.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gzduiiwum.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gunctvtlu.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gceabxbuf.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gbnbvxjvt.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gopggjcol.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gxgzuvbfk.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gkoxsbciw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/grnhbzycx.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gvpxikxfp.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gcfwmmvzs.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gcrwkneko.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gksatfrtb.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/grpjofgih.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/ggipoypny.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/ghttascqn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gdhejobiy.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gezouehkl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/ggvxftmbj.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/guomgpnue.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gfiqamrwx.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gfchcahoi.sHtML


<!-- 参考信息 -->