代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yvedp.cn/gtwfwehkgj.html

[Q24] 去重
来源：http://hz.jinqigfzy.top/gtptkjoqgn.html

SELECT DISTINCT city FROM users;
来源：http://hz.yongpay.top/gtbluuklwu.html

[Q25] 只取前 N 条
来源：http://hz.iojbl.cn/gtvttoeqwq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.daria6918.cn/gtpaotfpux.html

[Q26] 计数
来源：http://hz.jqgufenzy.top/gtpefubnzs.html

SELECT COUNT(*) FROM users;
来源：http://hz.feifeiyinyue.top/gtytnxmuxu.html

[Q27] 条件计数
来源：http://hz.mhx1999.top/gtfhdaueco.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cqqwz.cn/gtyzrdrgic.html

[Q28] 求和与平均
来源：http://hz.sxryk.cn/gtqvzlosih.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.meibo888.top/gtxwbnkhrs.html

[Q29] 最大最小值
来源：http://hz.xylfe.cn/gtcvshmhyj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ehwqpu.com/gtamczldod.html

[Q30] 分组统计
来源：http://hz.wangdashe.top/gtaglqezpl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtwqigluiw.html

[Q31] 分组后过滤
来源：http://hz.zhoulong.xyz/gtzwhakxeo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shanyushiyangtech.top/gtvtiqmhkf.html

[Q32] 分组拼接字符串
来源：http://hz.hongshengwenyu.top/gtoxyjwkgp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtznwbttpz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xuetiantiany.cn/gtgaykrswy.html

[Q33] 多列分组
来源：http://hz.gzhubu.top/gtctinndws.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.316326.xyz/gtjjjbdgce.html

[Q34] 每组取第一条
来源：http://hz.jiagoushi.top/gtgfvuqaxb.html

SELECT * FROM (
来源：http://hz.pycfn.com/gtgjfvotrp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhaomingkeji.xyz/gtymyosptp.html

) t WHERE rn = 1;
来源：http://hz.shanyushiyangkeji.top/gtljwzzwkg.html

[Q35] 内连接
来源：http://hz.ydjk.org.cn/gtdzukpmxs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.9152youxi.cn/gtptyyezes.html

[Q36] 左连接
来源：http://hz.svipenyu.cn/gtbfsncvuu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zycfv.cn/gtdsevilhj.html

[Q37] 右连接
来源：http://hz.pengpengdd.cyou/gtfskzjrtf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hysaishi.cn/gttybngktw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.haohaochexian.top/gtxzicrjsq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gogol.net.cn/gtehifvnkz.html

[Q39] 自连接（查上下级）
来源：http://hz.mhx1999.top/gtddwxdnob.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shanyushiyangkeji.top/gtgcmeejge.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shanyushiyangkeji.top/gthjwbdlld.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ywan-chungtsiang.top/gtcllsqgfh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.haohaochexian.top/gtouklwmmw.html

[Q41] 多表连接
来源：http://hz.daxiang520.top/gttctixxaa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.snrcjt.cn/gtfttwmrij.html

JOIN users u ON u.id = o.user_id
来源：http://hz.52xcode.cn/gtvvvwyflv.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.c1oappe.top/gtltaohjja.html

[Q42] 连接条件附加过滤
来源：http://hz.nwbrower.top/gtmzrncbbg.html

SELECT u.name, o.amount FROM users u
来源：http://hz.daxiang520.top/gtagijeqea.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangshuangyany.cn/gttmckfdgz.html

[Q43] 标量子查询
来源：http://hz.gzhubu.top/gtjvcsdrwt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.fengsongda.top/gtgbyigrhq.html

[Q44] IN 子查询
来源：http://hz.andypj.xyz/gtalqszvhb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.iojbl.cn/gtehsvbwhk.html

[Q45] EXISTS 判断存在
来源：http://hz.kuanghao11.cn/gtisbjnybk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.smart0.xyz/gtivnbdctw.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xziqi.cn/gtlogfrbvs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tian-w.cn/gtmrumbgxj.html

[Q47] 与平均值比较
来源：http://hz.tianlin.xyz/gtwnuogqxx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenzaomai.com/gtjtahjlbs.html

[Q48] CTE 公用表表达式
来源：http://hz.feifeiyinyue.top/gtrgwqjsnb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cheryme.top/gtobgkvrqm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.pengpengdd.cyou/gtlpjtvofv.html

[Q49] 更新单行
来源：http://hz.havefunace.top/gtamjqnope.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258.top/gtlhrbuusz.html

[Q50] 批量更新
来源：http://hz.tianlin.xyz/gtpeqwyufs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hywenlv.cn/gtsqrezkyy.html

[Q51] 用子查询更新
来源：http://hz.birdmap.top/gtuwcijqmc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.havefunace.top/gtvdqqictk.html

[Q52] 删除指定行
来源：http://hz.kuanghao11.cn/gtkpruygik.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zycfv.cn/gtzvsnzagy.html

[Q53] 按条件删除
来源：http://hz.daria6918.cn/gtlpjaexhi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jqgfzy.top/gtgxjyncvp.html

[Q54] 清空表
来源：http://hz.feifeiyinyue.top/gtilogrplu.html

TRUNCATE TABLE logs;
来源：http://hz.zdqjudy.top/gtpudifemp.html

[Q55] 排名（并列占位）
来源：http://hz.zhaomingkeji.xyz/gtrnbonthz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yuxming.cn/gtmspnyrkd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.9152youxi.cn/gtmrpzfvdr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.meibo888.top/gtzkrkwevx.html

[Q57] 行号
来源：http://hz.ivvv.top/gthsbqfeek.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shuidangran.top/gtqgfyntma.html

[Q58] 累计求和
来源：http://hz.316326.xyz/gtfbtkndgs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cqqwz.cn/gtrqrbmfaz.html

[Q59] 分组内累计
来源：http://hz.aibaodan.cn/gtyqtqigqn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.snrcjt.cn/gtpydwxlct.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhixingplan.top/gtulpshuxd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.316326.xyz/gtjqbzxmxa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zdqjudy.top/gtiwzaffee.html

[Q61] 移动平均
来源：http://hz.vqdsnc.cn/gtbdusvqjo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.bjfxy.top/gtudoyoaal.html

[Q62] 分组占比
来源：http://hz.yanxiufei.cn/gtunevnspp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ydzc1.top/gtqwovyhiq.html

[Q63] 开启事务
来源：http://hz.chenzaomai.com/gtlzexvavg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.snrcjt.cn/gtxunsrxan.html

[Q64] 提交事务
来源：http://hz.zhijiandao.cn/gtikscwabh.html

COMMIT;
来源：http://hz.ppjwa.cn/gtaumpviko.html

[Q65] 回滚事务
来源：http://hz.dashuyun.cn/gtgxgwlvnv.html

ROLLBACK;
来源：http://hz.sxryk.cn/gtqybxmkma.html

[Q66] 行锁查询
来源：http://hz.jinyuanbaomall.cn/gtcynxghze.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhixingplan.top/gtuhagevxj.html

[Q67] 设置隔离级别
来源：http://hz.havefunace.top/gturecndxg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.aibaodan.cn/gttthimlom.html

[Q68] 保存点
来源：http://hz.hongshengwenyu.top/gtjrparmhn.html

SAVEPOINT sp1;
来源：http://hz.cqqwz.cn/gtmjcbijrm.html

ROLLBACK TO sp1;
来源：http://hz.ivvv.top/gtkyybytxt.html

[Q69] 查看执行计划
来源：http://hz.nwbrower.top/gtsujqicvq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gotoacloud.top/gtrvqhfkge.html

[Q70] 更新统计信息
来源：http://hz.yuanzhike.top/gtpsnrzjzj.html

ANALYZE TABLE users;
来源：http://hz.gogol.net.cn/gtwzhqwlop.html

[Q71] 查看建表语句
来源：http://hz.hammf.cn/gtwmuhofqe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.feifeiyinyue.top/gtqsbxgwrg.html

[Q72] 查看索引
来源：http://hz.sxryk.cn/gtwuikknnl.html

SHOW INDEX FROM users;
来源：http://hz.birdmap.top/gtgboiznbo.html

[Q73] 查看表状态
来源：http://hz.pycfn.com/gtdmxiutyb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj20258.top/gthcgvujpf.html

[Q74] 强制使用索引
来源：http://hz.hongshengwenyu.top/gttvzuewbz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ivvv.top/gtenheizut.html

[Q75] 日期格式化
来源：http://hz.dianchejie.cn/gtxulldyuf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jyoumei.cn/gtqodwrwza.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xuetiantiany.cn/gtfmzmxmdh.html

[Q76] 按天统计
来源：http://hz.fengsongda.top/gtoiblsgth.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jyoumei.cn/gtopquivak.html

[Q77] 时间加减
来源：http://hz.zhixingplan.top/gtsphlhxge.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.aibaodan.cn/gtejquykvy.html

[Q78] 当前时间
来源：http://hz.gotoacloud.top/gtxnntqore.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinqigufen.top/gtkyhzmpmi.html

[Q79] 字符串拼接
来源：http://hz.yueranfly.top/gtavzvxpti.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ydjk.org.cn/gtusdcywyt.html

[Q80] 字符串截取
来源：http://hz.xuetiantiany.cn/gtijivyuid.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.kuanghao11.cn/gtmsfvraec.html

[Q81] 字符串替换
来源：http://hz.0kj1m.cn/gthlkymzfj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.haohaochexian.top/gtsxlyzstd.html

[Q82] 字符长度与字节长度
来源：http://hz.jinqigfzy.top/gttcrftont.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtliiqkxuw.html

[Q83] 大小写转换
来源：http://hz.jinqigufen.top/gthmprryjh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtsrynsgop.html

[Q84] 去除首尾空格
来源：http://hz.52xcode.cn/gtkivhhoxw.html

SELECT TRIM(name) FROM users;
来源：http://hz.jqgfzy.top/gtetyvzrnh.html

[Q85] 数值取整
来源：http://hz.hongshengwenyu.top/gtzbzsbupo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.fengsongda.top/gtedmazpzs.html

[Q86] 读取 JSON 字段
来源：http://hz.chenjidiqi.icu/gtosqsgqgi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shanyushiyangtech.top/gttcsppodm.html

[Q87] JSON 字段做条件
来源：http://hz.shangyingyoupin.top/gturdcrhfq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ehwqpu.com/gttieydmur.html

[Q88] 行转列（条件聚合）
来源：http://hz.feifeiyinyue.top/gtpgimerwv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhixingplan.top/gtxudbowwb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.dashuyun.cn/gtfzfqhvhv.html

[Q89] 判断表是否存在
来源：http://hz.hysaishi.cn/gtuuepljtd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.aibaodan.cn/gtuheqyoaw.html

[Q90] 生成序号列
来源：http://hz.yuxming.cn/gtfqnaayeg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ydjk.org.cn/gtcqctyxce.html

================================================================================
来源：http://hz.xziqi.cn/gtugocwtvh.html

R. Bash 专题
来源：http://hz.jianghu66.top/gtsutfmris.html

================================================================================
来源：http://hz.316326.xyz/gtfwfqdbhi.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangtech.top/gtdipxfzyk.html

#!/usr/bin/env bash
来源：http://hz.c1oappe.top/gtrwtxdvxi.html

set -euo pipefail
来源：http://hz.daria6918.cn/gtyxjvhyfr.html

[R02] 变量赋值与使用
来源：http://hz.gzhubu.top/gttrapidpm.html

name="Tom"; echo "$name"
来源：http://hz.guowangkeji.top/gtjjegtyef.html

[R03] 只读变量
来源：http://hz.ydjk.org.cn/gtkkdmmcqq.html

readonly PI=3.14
来源：http://hz.xingfuxueyuan.xyz/gtzjpqdihd.html

[R04] 位置参数
来源：http://hz.gaohongyu789.top/gttfzvujto.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xuanzx.com/gtualqpbnz.html

[R05] 参数默认值
来源：http://hz.yuanzhike.top/gtespzhunj.html

name="${1:-default}"
来源：http://hz.yongpay.top/gtykhlewhk.html

[R06] 判断命令是否存在
来源：http://hz.daria6918.cn/gtypfzftkr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sysykeji.top/gtqxxtzxhu.html

[R07] if 判断文件
来源：http://hz.jqgfzy.top/gtaiidnqpw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.nanxinkj.top/gtztjhyrgg.html

[R08] 数值比较
来源：http://hz.vqdsnc.cn/gtdfftzddv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gzhubu.top/gtgkakxenk.html

[R09] 字符串比较
来源：http://hz.cashguo.top/gtaevjtiav.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sufxvd.cn/gtlrvhfzfe.html

[R10] 正则匹配
来源：http://hz.jinyuanbaomall.cn/gtehgrusrf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shanyushiyangkeji.top/gtnolikrer.html

[R11] case 多分支
来源：http://hz.316326.xyz/gtyzzrjbrs.html

case "$1" in
来源：http://hz.aizwys.cn/gtzbdvvkfa.html

start) echo "启动" ;;
来源：http://hz.jinghuilouyu.cn/gtkdkheiab.html

stop)  echo "停止" ;;
来源：http://hz.jqgfzy.top/gtwjkrfhir.html

*)     echo "未知命令" ;;
来源：http://hz.chenzaomai.com/gtfxwvybhj.html

esac
来源：http://hz.cashguo.top/gtwnltkymt.html

[R12] for 遍历文件
来源：http://hz.cqqwz.cn/gtzzttnkfj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jianghu66.top/gtjjgrqyxd.html

[R13] for 计数循环
来源：http://hz.xuetiantiany.cn/gttpmynpip.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gaohongyu789.top/gtlmhbmwfl.html

[R14] C 风格 for
来源：http://hz.hnqzz.top/gtrrxqzrmq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ydzc1.top/gtpycxgyak.html

[R15] while 逐行读文件
来源：http://hz.yuxming.cn/gteskaenfg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.birdmap.top/gtceozwkli.html

[R16] until 等待条件
来源：http://hz.jlsjyb.cn/gtwuspkqwv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yongpay.top/gttfodrjpb.html

[R17] 数组定义与取值
来源：http://hz.ybcxt.top/gtpanpfwic.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.c1oappe.top/gtecdlwgcd.html

[R18] 遍历数组
来源：http://hz.hammf.cn/gtprvzbhhc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.pycfn.com/gtheubfhqg.html

[R19] 数组长度
来源：http://hz.cdnleiting.top/gtirjkzdan.html

echo "${#arr[@]}"
来源：http://hz.guannengcc.top/gtmpnlogjo.html

[R20] 关联数组（字典）
来源：http://hz.zdqjudy.top/gtbsquknco.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhaomingkeji.xyz/gtuhbqtujp.html

[R21] 字符串长度
来源：http://hz.quarkkingdee.top/gtodkrwakf.html

echo "${#s}"
来源：http://hz.ppjwa.cn/gtqifwvcyq.html

[R22] 截取子串
来源：http://hz.haohaochexian.top/gtueicgrow.html

echo "${s:0:5}"
来源：http://hz.jyoumei.cn/gtzmyarpdu.html

[R23] 字符串替换
来源：http://hz.dianchejie.cn/gtvsbttmeh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.chenjidiqi.icu/gtjgdlwghq.html

[R24] 大小写转换
来源：http://hz.9152youxi.cn/gteyavipoz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.iojbl.cn/gtbwmgqudo.html

[R25] 去后缀 / 去前缀
来源：http://hz.cashguo.top/gtsmbbdldd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yuxming.cn/gtuwoxppuk.html

[R26] 命令替换
来源：http://hz.yj202588.top/gtsilhxcmq.html

now=$(date +%F); echo "$now"
来源：http://hz.wangshuangyany.cn/gthzdjyqhl.html

[R27] 算术展开
来源：http://hz.mhx1999.top/gtuvchdhqo.html

echo $((1 + 2 * 3))
来源：http://hz.nwbrower.top/gtmlfqzxup.html

[R28] 浮点运算
来源：http://hz.chenlongwang.top/gtyumipzan.html

echo "scale=2; 10/3" | bc
来源：http://hz.ivvv.top/gtifdxgonk.html

[R29] 定义函数
来源：http://hz.pycfn.com/gtvoyroshw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hysaishi.cn/gtmhatyhbw.html

[R30] 函数返回状态码
来源：http://hz.guannengcc.top/gtsbqmzzvr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhongyouzk.top/gtgivuuvhi.html

[R31] 局部变量
来源：http://hz.jqgufenzy.top/gtzvovcizo.html

f() { local x=1; echo "$x"; }
来源：http://hz.gotoacloud.top/gttvtddlry.html

[R32] 参数个数校验
来源：http://hz.jinyuanbaomall.cn/gtnbyhbcna.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.iojbl.cn/gtadmemrai.html

[R33] 捕获错误并提示行号
来源：http://hz.bjfxy.top/gtavcapdkh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hnxiangtu.top/gtxrhxadlt.html

[R34] 退出时清理
来源：http://hz.cqqwz.cn/gthkhtxewt.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hongshengwenyu.top/gtkmcxfnhn.html

[R35] 后台执行并等待
来源：http://hz.dianchejie.cn/gtibkhpsgs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hammf.cn/gtauezqbfx.html

[R36] 并发执行多个任务
来源：http://hz.redwolf501.top/gtcheilecl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ppjwa.cn/gtpimeyioh.html

[R37] 把输出赋给变量
来源：http://hz.yj20258.top/gtoharxifr.html

files=$(ls -1)
来源：http://hz.quarkkingdee.top/gtocjjunbi.html

[R38] 管道串联
来源：http://hz.yj20258888.top/gtygdridsz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.redwolf501.top/gtnhayorpr.html

[R39] 重定向标准输出与错误
来源：http://hz.vqdsnc.cn/gtosanjvzj.html

cmd > out.log 2>&1
来源：http://hz.pycfn.com/gtgtmnmkan.html

[R40] 追加写日志
来源：http://hz.ybcxt.top/gtnhogzzgb.html

echo "log" >> out.log
来源：http://hz.yj202588.top/gtdltsswab.html

[R41] 丢弃输出
来源：http://hz.fzhhl.top/gtwbouqdyy.html

cmd >/dev/null 2>&1
来源：http://hz.zycfv.cn/gtbeiwiney.html

[R42] 输入重定向
来源：http://hz.ybcxt.top/gtjmitdzep.html

wc -l < a.txt
来源：http://hz.sxryk.cn/gtuezjljpu.html

[R43] 按名字查找文件
来源：http://hz.pycfn.com/gtxuqmtqeq.html

find . -name "*.log" -type f
来源：http://hz.c1oappe.top/gtswuxucry.html

[R44] 按修改时间查找
来源：http://hz.yuanzhike.top/gtfyecmolo.html

find . -mtime -7 -type f
来源：http://hz.xziqi.cn/gthphzyevy.html

[R45] 批量删除
来源：http://hz.ppjwa.cn/gtpibagmwq.html

find . -name "*.tmp" -delete
来源：http://hz.bjfxy.top/gtoswluxrl.html

[R46] 递归替换文件内容
来源：http://hz.andypj.xyz/gtfuyngcwe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shzxlz.cn/gtfteywadj.html

[R47] sed 单行替换
来源：http://hz.zhijiandao.cn/gtbrilqfkf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.9152youxi.cn/gtswhgrdgf.html

[R48] awk 取指定列
来源：http://hz.bjfxy.top/gtdgelajri.html

awk '{print $1, $3}' a.txt
来源：http://hz.svipenyu.cn/gtzfigtfbw.html

[R49] awk 带条件
来源：http://hz.dashuyun.cn/gtjmrbtklo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jianghu66.top/gtrfscdgwf.html

[R50] awk 求和
来源：http://hz.cashguo.top/gtepzbbamz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cdnleiting.top/gtymkjpboa.html

[R51] 排序去重取前几
来源：http://hz.jinqigufen.top/gtxbyfkzmu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hywenlv.cn/gtyggsfjlb.html

[R52] 统计行数
来源：http://hz.fzhhl.top/gtflpjizet.html

wc -l a.txt
来源：http://hz.smart0.xyz/gtdfjqtxpv.html

[R53] 查看文件头与实时尾
来源：http://hz.nwbrower.top/gtujopfuvg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cqqwz.cn/gtfewdwjty.html

[R54] 比较两个文件
来源：http://hz.xuetiantiany.cn/gtqwqrbaed.html

diff a.txt b.txt
来源：http://hz.tanke756.top/gtzstbqwjd.html

[R55] 压缩与解压
来源：http://hz.chenjidiqi.icu/gtiimhbxjj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yueranfly.top/gtdpypejqr.html

[R56] 远程拷贝
来源：http://hz.yvedp.cn/gtkozwlurt.html

scp file user@host:/path/
来源：http://hz.pycfn.com/gtvzxndago.html

[R57] 远程执行命令
来源：http://hz.tian-w.cn/gtrhkrvqmp.html

ssh user@host 'uptime'
来源：http://hz.9152youxi.cn/gtwwggmnyq.html

[R58] 下载文件
来源：http://hz.zhixingplan.top/gttdbodpdk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jqgufenzy.top/gtonzapisw.html

[R59] 发 POST JSON
来源：http://hz.jyoumei.cn/gtimsfssyt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.andypj.xyz/gtkqvjmdtf.html

[R60] 只看 HTTP 状态码
来源：http://hz.tian-w.cn/gtcueenqug.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tanke756.top/gtbmbuxpkk.html

[R61] 磁盘占用
来源：http://hz.tanke756.top/gtmyqnoihr.html

df -h;  du -sh *
来源：http://hz.smart0.xyz/gtnrytrchb.html

[R62] 找最占空间的文件
来源：http://hz.nwbrower.top/gteaokctqj.html

du -ah . | sort -rh | head -10
来源：http://hz.ydjk.org.cn/gtayjjotug.html

[R63] 内存与进程
来源：http://hz.zhiwuduotai.top/gtxkiffgjv.html

free -h;  ps aux | grep nginx
来源：http://hz.wangshuangyany.cn/gtfqxgsgmf.html

[R64] 结束进程
来源：http://hz.smart0.xyz/gtuwpafepj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.52xcode.cn/gtjnambczl.html

[R65] 查看端口占用
来源：http://hz.zdqjudy.top/gtarsyjyuu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yongpay.top/gtqfadrsls.html

[R66] 定时任务
来源：http://hz.daxiang520.top/gtizbydmlh.html

crontab -e;  crontab -l
来源：http://hz.snrcjt.cn/gtombwoioy.html

[R67] 生成随机十六进制串
来源：http://hz.zhoulong.xyz/gtxzxzhbpm.html

openssl rand -hex 16
来源：http://hz.ppjwa.cn/gtgrqzvczi.html

[R68] 计算文件校验值
来源：http://hz.52xcode.cn/gtmmvqtdwr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gaohongyu789.top/gtcizienru.html

[R69] 生成随机密码
来源：http://hz.jlsjyb.cn/gtwyxnyfzp.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhengqikj.top/gtszxwukqr.html

[R70] 时间戳与互转
来源：http://hz.ivvv.top/gtqabzbkwy.html

date +%s;  date -d @1700000000
来源：http://hz.ehwqpu.com/gtjnisqizj.html

[R71] 日期格式化
来源：http://hz.xuetiantiany.cn/gttoccrege.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinghuilouyu.cn/gtucyqkhtq.html

[R72] 等待端口就绪
来源：http://hz.shuidangran.top/gtzhywahzu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.dianchejie.cn/gtxzgcugga.html

[R73] 分割大日志
来源：http://hz.hfpthk.cn/gtdvbmsmcm.html


<!-- 参考信息 -->