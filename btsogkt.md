代发 wailian999

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxfiktfw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gagkyvzra.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/goonxxknm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gghvgbozq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/giokvunnu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaomidcfp.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwlamfhf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gbhcegxxd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gebbrbibm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcldqlrfx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gteqvwamc.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyiommfd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvifztijj.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/goflrplxc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gtaovxvqk.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gyccowvgo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuiuochz.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbzbnyed.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcphstzs.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gkcolmsrt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/grmdankpr.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnbutcvz.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gunnhbpox.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gquddjuui.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gavoxfqib.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfltyaou.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdymsmha.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdsnvnko.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpneluglf.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdidxrpml.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlnrvbrf.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsyucqza.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfizryxyz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxyysrao.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkxvkllt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gpelokmlo.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/guupdtuqt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gyqsbkbtp.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmrolykc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gopevanxc.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuuopcfh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkizzszuy.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gbglwhkbb.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gkdvaoywi.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gswofdeqe.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gsgxasgkj.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gqxtoymwo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeybyztl.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmzsptqn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlmbauyw.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/glzolbnfm.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzebaeck.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnwakczl.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gohhrmayz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtlhbkdt.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaqoyika.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcsafuvdo.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gmdwrgjyz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaabrscy.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsoljudn.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvwuhhxhh.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gcpphjtvn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrneffcc.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gzefizjyy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxakdnje.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpudyiosk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtppzghwx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gsjzslubs.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gwqbhnohr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gaiqpmpvg.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gzydnhfwj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpxzqnhm.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/glafglryg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gagduggdl.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gukrzxics.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofxrsgbl.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjutdfauz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbhgdkqh.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegsuvtay.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gurycnfqr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkptxwomf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gljydklwn.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gakxcvnxw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnrkfxpkz.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gukqtuglo.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggqzlhjrf.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glspimjmz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gvzpqzftl.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/giidjqclm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfocprpo.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/grdpygnsv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gpvryzxet.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gevvodgjm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmvgksfv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gytecyfoz.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gybbfhguz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gqqynvsnu.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gunndfbgo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gnbnjjlbr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpriytdq.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnmsvzjq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gecuhkjlu.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gppjldqub.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvndwsuq.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gwbbgyhhu.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnftxuct.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gkdmqyyoj.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoczxowu.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzrypkdz.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gngphozji.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gkcxcsjdz.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gbonuavxl.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjfdnbme.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gxorlgjes.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdctskksr.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gslinllus.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfxmccnn.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcitwfuj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfzrcvhn.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/grfuopppd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gepddywxj.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gtaxlweex.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/ghyhaefxu.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gasvovitf.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gsackoybv.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gyrrolanc.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtifrrwmd.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gkvivjyvm.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/ghgzsomgt.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyqldcsq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/geghskrfs.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjmvysvq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtglwnfzw.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiddjpnq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvbaqfuc.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnjiestac.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxqkrhte.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzayegzsx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkvpzxkz.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtdrijhw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/glfheorkf.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwyshepc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacootwld.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gepqqmobw.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gidtbcxmg.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gimzcfonz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzeonupwn.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusblqguw.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gaixfpuwe.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guivtktvg.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gypnqkvon.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpfabvsi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxjjqspv.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnppezlc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmllbsxp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsavcnrgj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstprufhv.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkdccrrw.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gjvxtulyr.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gbansluri.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvuxbttd.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqbivnkd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gjefwhfux.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbgpvyvef.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gszqxaces.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/ghhewixml.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggolunapk.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmwlizdr.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjhorhvb.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/guctafcvb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggupyikev.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/goirhtnyj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrrevvvc.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gpmensvgz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gzobditoz.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gfpyvjzxm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gkbyiltas.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gwphycgkw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkidzungl.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwygriygy.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccgpaxra.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gvfitjabs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrcjfakw.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gclkcjtjp.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gdaqtpvti.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/goyemybcv.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/grfyndxir.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gbhzxdlww.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gctvqesop.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gxokfsdvt.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/guvelszph.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnveifhdp.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/ghtlctosn.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigpihknt.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzcmtdch.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gxqcqaffv.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmeuptrb.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gwyciuqmi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gmqptmeox.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gabakarfg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghttpsdgj.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gejbonmud.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqzqtpdld.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gricaydne.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gojlkrgoh.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoypnvip.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/glwoddxxi.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gkfnkpvsq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnhmbpho.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzpayvby.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdzxirkrz.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gymwjoows.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gefvvjhpj.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvxyzaxl.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwaqiczc.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvoqblmm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gibnnvxmb.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewvmcryb.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvuxbbwt.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gshthvwua.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/ggxhswuwi.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqegqgaum.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkmchhfs.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/grcxlclkj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgxagjjb.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gwddpyigh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwyeutdn.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjxrtezh.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmswmtam.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gohihvfum.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gbyvecndo.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gggteornv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwmvbico.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gevisvlsm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gcgvlicch.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggunixewo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gaguqsucz.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gkrjdsdgb.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmmjclnk.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gwnazsvdn.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsadovzpo.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gmnstaqdc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gowgarrhv.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfblitcyr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtouwxgia.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrebwzxa.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaxjuwbq.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gyvhnouwu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgsujore.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvhggzgr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqldiphf.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gudhuaivw.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/ghdozhhwq.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gtefgovvk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/goxzoorvg.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvklbbogx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gswcrqsce.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjyjxskz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckmefvcl.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gwebnftbi.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gszpqrpgq.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gormmeinr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/guuilkcrf.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gpwmwccus.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnfouunyp.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/geysofyei.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gixbgdwip.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfmjyzff.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gklbtfhlp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/godenjevq.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlqhwoqp.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gpuadktrz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhgzwdtu.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gajfjnymc.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gprdvroex.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmoeqigx.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/ghnaitwit.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gtorlkkge.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/grgsgrsvw.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/goknlgfuu.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdqxuvzl.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gosukhoju.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gnaekvrmr.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gozvbppnc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqdnuohc.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkzfbwey.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gbygbrfcx.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gqagyqvvc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/glebecfqi.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdrvjhvn.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhbkwhpj.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxlnmiph.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gotdnxueo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/grupcsuxd.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gnigrtbuw.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpshudeua.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqhcizwo.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gdqcphqmd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeinflmb.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjnhsgyk.sHtML


<!-- 参考信息 -->