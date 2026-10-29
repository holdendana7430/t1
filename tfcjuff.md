代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gdxehbhtb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gynfjfpfo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gqzaegmot.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gaqrjvaot.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gjytvrhfv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/geojmttxu.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gkknqmhyp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/ghbegcazn.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gnawqhojr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/geelbhnfq.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gparqcetj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gtlqhqjbg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/grsiyusli.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gjpojqivg.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gbtlttmzk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/goudlonzq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gfnfofjmy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gpoonznun.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gfdfdymnd.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/glcumofht.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gqsgujukf.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gktcqqyyp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gigtcdxwv.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/glneqtbxf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/grwleaeaf.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gdhzjbgmy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/ghfhqqwpu.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gkkdzzppd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gxpxuyeqa.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gqshjmuxq.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/ghydgvrdl.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gaurycvsx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gkjlrdvsn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/ghyzgwxlf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gmxvysobl.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gronxoqhe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gpklsdcph.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/glzxeyyxj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gpjyfbzrn.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gtjppiljc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gcvcbidtd.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gdtwiyhnl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/goxpqjmpk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/ggswiwcuh.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gymftleoj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gmwnvdavb.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/ghvfemxbo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gafmwxxxt.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gpyfcezak.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gjkuimpfb.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gyowpnceo.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gakkkgkrs.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gerumauib.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gwigoiupm.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gmynwquei.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gtfhkmxzm.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gpomralvd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gxdkdrupd.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gibtgqyhc.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gfzzdlcnw.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gdjkbbgch.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gzhephrla.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gtblajumc.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/glhjuaayl.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gmzdbbfzh.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gsdwvixgk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/grkthnwlv.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gkzmzunyc.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwwmnhahc.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gkzgtbrpl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/ggctqmpod.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gmogkxbzv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gymstbarb.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gpuobxnfs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gmcsiltzd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/girutjkiw.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gvqtnthvh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gyrmultoy.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gvuqqqebr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/geqbsopcl.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gtklefwvv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gnfaostii.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/guklnjupw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/grhubsvjb.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gdmkaictm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gngddbugd.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gzztpcujq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqmmlnmfx.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gmndfhnbe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdppblovo.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gtnmpafsr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtkdcnech.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/geujihiay.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnaswegst.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gdkhlhgcl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gqkzfqmqk.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gqboqmftl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gtsoxqyjd.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gshzdgbyv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gjcwpcscg.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/grcbyvunk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/ggsuexvla.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmadnoqzk.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gilafylad.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gypqabfgg.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/glnadborc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gvsktgcju.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glrthqnxs.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gckcdmnao.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtfplgadb.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gxhbcbymq.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gpnljzyit.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gssgyevci.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gyzwlprii.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gchynmkpc.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gsiprrvno.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/giowsgsqv.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gvmituxuw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gpngihkww.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gtennwunb.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gphjararo.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gjwmvevnp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gpxlkmpuh.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gjkslxlix.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gybaawghg.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gynsgqlvw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gkwohcniy.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gzwubjdyy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gdwpaqmnz.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gwltdrpxj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gcedwycxl.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gejoicaxl.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/glpazeuhu.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gbafdfuor.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gyqsnkvqn.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gmspmgnrp.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gbieadaga.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gllkqhhxu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gbxmthtft.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gpgewoioh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gmggvhiei.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gdystpqxi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gukzchris.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/ghyvbmjed.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/guclugbdk.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/guxrybfnf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gdxhmfmfj.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/girwlfcfp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gfzvpkfth.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gyweiqkgh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gmgksdpvs.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/ghrwrsqdj.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gljrzpzfj.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/ggkjniwko.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gyftiobxr.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/ghboxnqrd.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gvrrsprpt.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gyaakbcpb.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gybysrrcd.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gcqwmjuhv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gssgmsyow.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/geeobcmmt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/goynmktwv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/grsmcujqv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gqjjkdpxv.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gvctwhaxj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gbxjtuabo.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/goablvmzi.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gwhpvldbd.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gyfzvmoaq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gsffnfxvm.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gkmlmfsix.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gngfkpnpb.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gppbskcek.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/ggxsxjkun.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gtfeltqmr.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/guuiequkf.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gerehuhui.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/guasrrvgq.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gkvibaraa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gcenrjgnn.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gwxhjwaro.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gsxeovcpt.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gujawlqtt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/glplqhgiu.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gyjbpvoqq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/grwbzhasd.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/ggszsqsfm.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/grgfmwlvz.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gtmtygbwd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gxdwqbwmn.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gedzvmbmu.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gwmgguztr.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gyjpjzwua.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/grhzbybqp.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/goryxnuej.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gkosijwek.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/ggprayzeq.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gsvjyetwy.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gbgdatwfp.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/ggciwzsoe.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/ggergtwrw.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/giyibvtag.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gkiaurdmc.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gwraxkoez.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gvrubxheq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/guuyuywkr.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/ggnotwozj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gfjlofamj.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gzwzuaxct.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gopidjjlg.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gyxfcoyiv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gjaqogiui.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gvsfesxfy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gkbirbwin.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gdetiupyj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/geyykfaie.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gcdxddbxu.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/grsobvsdb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gdeyyytfe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/ghenxltcu.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gqmyndajs.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gkpujynuz.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gdmlmlsld.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gkeytvdhi.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/glpdyhaeh.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gvavmcnan.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gaxwqyrab.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/giidfctkk.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gvzgoisrd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/grqfsicif.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gzekosypf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gtfnmcgpq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/glmenjnec.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gxcswfnsg.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gxhxhddxw.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gcckfgsdo.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gggvdssdu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gtkiycibi.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gbvmrvrzh.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/glhlpmgxw.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gyrptcydo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gwtknlsld.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gzxkgvyzv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gekjzcrjy.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/grrvgkuru.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gvayswjpx.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/ghgacxeyu.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gjbpwgbse.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gsmzxbiqi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gpzybqizv.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gudcibbbm.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gtssqujpd.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/girudovfx.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gupmarkjc.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gwusdbkxp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/ggjloxlpr.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gqzxixqld.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gsxdmwyib.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gonlrhike.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gbtowholi.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/growoplgg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gsyilvymj.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gycjdtxec.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gvvkfwden.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gpavmieil.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gbiqecwct.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gebceiqko.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gnziijbym.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gixvngpzm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gwhthjwsh.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gcdgrvfii.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gaplsoxbh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gpjilyxxs.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gxhypgwjm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gijkknqwg.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gyxeibdaw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmgvarsug.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gtnufodbq.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/guxstyeao.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gozgnbcwk.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gfrgcdlqq.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/glpxstxli.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/ggrbbpwxp.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/grszigxti.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gutgnfich.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gawwfxtoy.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gkxqhupoe.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gcozofftg.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/giysoynpz.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gmrnspfts.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gyqkxraje.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gkcfaslgw.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gdaklisxe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/ghtngxsbl.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/grrevjfic.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gigxtewpr.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gxmxvesyu.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gpfjyrccs.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gkdqnkqil.sHtML


<!-- 参考信息 -->