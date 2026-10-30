代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gqokipbmx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gideasjnn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gvvicnhhk.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gjgieumyw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gujgohalt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gmiupserb.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gxiarojpj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gpkmhavzq.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/govkhskbw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gpiklylyi.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gcsipasdx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gtdtafpji.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gfwxznaaj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/glxgrhdnt.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/guyeaquhh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gfzjnvfem.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/ghaliegfl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gjgnoooun.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gzqieuqef.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gybfqdeyw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gvyhcyfpl.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gttsxlhzl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gfhmkorwr.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/grdjpfjvv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gwgtahfnp.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/glwqhpkdy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gohrxnxyu.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gyqrjqanx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/ghurmbgvd.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gdhczxell.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gyzfyknqq.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gkzsuegjq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/giffvndpw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gyjrubvpf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gldlsjtyy.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gqtigsidc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gcnpvarwj.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gjgykkwpa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gfvjtoihf.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/ghytpwglq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/ghktwwstx.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/glfwtqrha.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gomtzzcaq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gpvgliajm.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gkqocwwmf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gdpofssgg.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gdybwucfa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gkdsxhqxm.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gozdictpq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gpinojruc.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gpgbmgnnw.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gbfhcikwl.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gdspdzfws.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gomkhxcbe.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gijkevpuf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gvklzvrlr.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gokrvkkes.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gwsziqydb.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gsjkkwtzm.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gdimjiwkd.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gubaipddg.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/ghwzcyfhv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gomxypnno.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gcyouwkfy.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/goohesvts.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gxbssdkrd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gnikvbnbt.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/ggxokghwk.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/geqyumutb.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gqzpgjwph.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gfhgtlyng.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gsgcggnaj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gnbwhjmpl.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gxbxdnapk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gmalprvrk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/geqiinofg.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/geblyioys.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/ggoytdenj.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gvrkccrmt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gbkztuwhe.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gpqeohese.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gsxhocbaf.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gtmxnnstx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gziaugcio.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gxtibazpa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbjdqvzcf.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gcippytwe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gzlrtjtdt.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfpukvhqa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/ghxfnlnfs.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gpkbmlprh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmyawdzgn.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gdmytdato.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gghiihrdg.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gjiincrzc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gxuasdtkq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gzudwtcyu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gaikbfdfq.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gaoafhrfv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gkxlyqqeh.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gswexcunb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gqrvljpnu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gggrzxzlu.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gzlhipthk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gxlbldhov.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gmmtequsb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gtcnfdhdu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkrhzcecr.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gprbufmpw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkxzepste.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/ghsvghjma.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gkimramzm.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/ggmffhppu.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gkqwpsebd.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/ghfajjizo.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gohnpmjcg.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gctvbytes.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gjoqqkqyr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gaxpbijmo.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gfxxavxvg.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gktqokhio.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gsjlpdcop.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/grbauscgv.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gxwpalduw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gyurpgruh.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gbmpqmlqn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gqlkfzbqa.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gerljsbqc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/ggtotfxpt.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/ghbpibfrk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gfqlmbrzs.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gdjczfpll.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gecmnvaje.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/glsreetso.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gntsuubzf.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/giabhpevd.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gzusftfti.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gdildiwqv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gdpboskjh.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gkefknhhz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gqckufnzr.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gjidfprzg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/goikolxbh.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gzhkdxtgt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gjvmldadh.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gludumnxc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gvcjwaxwr.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gaafhwrka.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gcumbrryg.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/giegqazqj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gqbixweud.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gfpbgiyjj.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gixxgyygz.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gtrxxfomv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gwofjqsdb.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gbrotvpkn.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gnplncrqu.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gqfatewoo.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gywaecgmn.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gvuhwzeil.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gqzdddxzh.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gomqwehmg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gzeclaaws.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gkyorhoia.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/glcmamsyz.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gtgfsfnem.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gmvvpubyv.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gkmqiflsb.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gaowdcirl.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gjndxmdrz.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/ghmlbrrdc.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gedaquczq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gwyxwubiq.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gvqrmfqfw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/groncsibh.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gdsxldcyb.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gpdktvpig.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/ggyagnuej.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gxwxuritb.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gpzyaytyq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gptpvmwua.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gzdqpymzk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gcrwfnplt.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gpsuiprcs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gumromwmz.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gghcymxhg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gwgvzcxav.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gqpassvao.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gjruirxjv.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gaoabrrvr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gcnssdybb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gwqjwstra.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gsdnkjyjg.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gswbcakep.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gplemzluk.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gprqovhpk.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/guprjohry.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/goftuiekt.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghyvahgii.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gzbjdpoeg.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gdnjixluj.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gdamnpfsa.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gzwijmbmk.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/guusavifx.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/ggvbdvrhr.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gwonjsiee.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gcpklwryy.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gkzmyfgkf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gcdigxhxg.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gxqfytjpc.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gctbgujyc.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/grunteyvc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gzmbddgxi.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gblbgqkaj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gojnajbcf.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/goxqcwljf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gtdoiurhq.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gnkcnfpay.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gukvhdwty.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/godwkfkxj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gagbbduyx.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gaekokazz.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/givigelyc.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/grsnmufuo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gzjncvhab.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gtrfafxel.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gitalvoyc.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gmgxwqzwl.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gyhguuuza.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gncgcztpt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gbpvhfvue.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/ggfibnmop.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gcfnsoxpz.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/guorcbvzn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gsfqiwjxy.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gorozfibh.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gwcuywpem.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/grcmgsfro.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/glbqtvvnb.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gapqjdqtr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gwcjwtata.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gjprrpily.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gntttufcl.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/guxwmzqfv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gvqzqqlsu.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gjfiykuvf.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gfxvyggen.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gpocqgblt.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gjrroqubt.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gejgvkhxr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/glzsnnjff.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gwshifacn.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gvphoyibg.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/ghccchaaf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gnjjfdzeq.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gpiiaqvbt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gjbsjbmsl.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gblhwqzqm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/ghmvrhukj.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gdrdlqxli.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gooiuyuqb.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/giygalurk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gwqkamrwj.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gbpvfjbdy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gbfpcefhr.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gfrhzyjyo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gfxmtyccl.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gnspjcddt.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/ggfdjktkt.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gcnusotlj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gqcnftpsx.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gcwylhyyv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/giefalxkv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/goewvquto.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gralkuakm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gecjzngvu.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gvrfwbrdl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmwmubual.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gxebncrjo.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/glcyvtafe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gmmsacenr.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gofvuwufb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/guoxttfos.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/ghxecsdld.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/giuivhelw.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gcdnppynx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/glefbjqyy.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gettqplfu.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gcduhndio.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/glxzlygyy.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/glfqfvyig.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gwtidzrnx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gsxwoluho.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gqgygocxl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gmdyvhgzt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gnkospatl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gaixiwjds.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gipngojyw.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gobdrzfoz.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gvhpfbifr.sHtML


<!-- 参考信息 -->