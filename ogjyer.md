代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gaohongyu789.top/gthgeehsmo.html

[Q22] 排序
来源：http://hz.yj202588.top/gtlbmnmdlp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jiagoushi.top/gttkhcjfva.html

[Q23] 分页
来源：http://hz.zhijiandao.cn/gtpuqkgdxx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zdqjudy.top/gtjouunkja.html

[Q24] 去重
来源：http://hz.jyoumei.cn/gtvxzqiegu.html

SELECT DISTINCT city FROM users;
来源：http://hz.yueranfly.top/gtvgsfogkx.html

[Q25] 只取前 N 条
来源：http://hz.gaohongyu789.top/gtkimhlizs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shuidangran.top/gtxsqizhbu.html

[Q26] 计数
来源：http://hz.yangfankeji.com/gtpsdiddre.html

SELECT COUNT(*) FROM users;
来源：http://hz.meibo888.top/gtnwnmrpdj.html

[Q27] 条件计数
来源：http://hz.daxiang520.top/gtlhjubsxd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.0kj1m.cn/gtqxyqaado.html

[Q28] 求和与平均
来源：http://hz.dianchejie.cn/gtpxhicdtj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fengsongda.top/gtdshtfskz.html

[Q29] 最大最小值
来源：http://hz.gaohongyu789.top/gtkafvqcty.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gogol.net.cn/gtpsntekej.html

[Q30] 分组统计
来源：http://hz.yuanzhike.top/gtcbtvlsdn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtoqwyuqqd.html

[Q31] 分组后过滤
来源：http://hz.jiagoushi.top/gtxbwpplze.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.guannengcc.top/gtmzsixukf.html

[Q32] 分组拼接字符串
来源：http://hz.xinyue.icu/gtygvtbdvs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtpqyuiuel.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhoulong.xyz/gtyewoylzh.html

[Q33] 多列分组
来源：http://hz.shzxlz.cn/gtyugmlauy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shzxlz.cn/gthwivyaos.html

[Q34] 每组取第一条
来源：http://hz.havefunace.top/gtwrcbflji.html

SELECT * FROM (
来源：http://hz.zhongyouzk.top/gtezzfrzjr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.52xcode.cn/gthoxfgcgw.html

) t WHERE rn = 1;
来源：http://hz.andypj.xyz/gtnmpmjxbf.html

[Q35] 内连接
来源：http://hz.snrcjt.cn/gtldzhyups.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhaomingkeji.xyz/gtznpbggts.html

[Q36] 左连接
来源：http://hz.yuanzhike.top/gtwybhdyfb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.mhx1999.top/gtwydsapnz.html

[Q37] 右连接
来源：http://hz.sxryk.cn/gtklyijsuf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.daria6918.cn/gtlgporxjx.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hnqzz.top/gtrzmuolnk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.dianchejie.cn/gtldupuuuq.html

[Q39] 自连接（查上下级）
来源：http://hz.aizwys.cn/gthsokcxtd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yj20258.top/gtaoxuwujn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tian-w.cn/gtscbfgdik.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shanyushiyangtech.top/gtsyxsqwwi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hfpthk.cn/gtklfmotfk.html

[Q41] 多表连接
来源：http://hz.shuidangran.top/gtpniacbag.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.svipenyu.cn/gtwcwwelcs.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hongshengwenyu.top/gtqmeuirkf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sufxvd.cn/gteoivzlel.html

[Q42] 连接条件附加过滤
来源：http://hz.fzhhl.top/gthkolslrn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jianghu66.top/gtqlqxlmts.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.bjfxy.top/gtmppeijtr.html

[Q43] 标量子查询
来源：http://hz.zhongyouzk.top/gtbzmjltau.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yuanzhike.top/gtwpgpvwdw.html

[Q44] IN 子查询
来源：http://hz.vqdsnc.cn/gtuzgzgaqx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.mhx1999.top/gthyxqzsda.html

[Q45] EXISTS 判断存在
来源：http://hz.jyoumei.cn/gtxdmgtggx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ivvv.top/gtuecshfhx.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ehwqpu.com/gtswwwusvq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenzaomai.com/gtvbbyzmzg.html

[Q47] 与平均值比较
来源：http://hz.zhengqikj.top/gtimfmntpa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sweek.top/gtcybhunog.html

[Q48] CTE 公用表表达式
来源：http://hz.zhongyouzk.top/gtunyigkuq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jyoumei.cn/gthbudkujn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.daxiang520.top/gtcofdmxid.html

[Q49] 更新单行
来源：http://hz.smart0.xyz/gtbdtxilpb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.wangdashe.top/gtishrrlgn.html

[Q50] 批量更新
来源：http://hz.9152youxi.cn/gtswfkplwu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yj202588.top/gtjtgcutye.html

[Q51] 用子查询更新
来源：http://hz.52xcode.cn/gtxrejamka.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.c1oappe.top/gtuohuwhie.html

[Q52] 删除指定行
来源：http://hz.xylfe.cn/gtzczwjcwh.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zycfv.cn/gtkqlzgeac.html

[Q53] 按条件删除
来源：http://hz.sufxvd.cn/gtuinwuwzq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nwbrower.top/gtvyqnswqr.html

[Q54] 清空表
来源：http://hz.chenlongwang.top/gtjeqernse.html

TRUNCATE TABLE logs;
来源：http://hz.gotoacloud.top/gtwivvjwsj.html

[Q55] 排名（并列占位）
来源：http://hz.ywan-chungtsiang.top/gtmdpwqbrs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ydjk.org.cn/gtibmriodi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.aizwys.cn/gtfjwifqyh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.dianchejie.cn/gtisjivezv.html

[Q57] 行号
来源：http://hz.tanke756.top/gthhftpghk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.daxiang520.top/gtehprfvzk.html

[Q58] 累计求和
来源：http://hz.0kj1m.cn/gtabaxaxup.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.daria6918.cn/gtjvzcdfjj.html

[Q59] 分组内累计
来源：http://hz.316326.xyz/gtwkmxyqje.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.smart0.xyz/gtmpwnhqzs.html

[Q60] 取上一行 / 下一行
来源：http://hz.quarkkingdee.top/gtmpjeyawl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sufxvd.cn/gtywwdqzeh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.nanxinkj.top/gtorbtqrto.html

[Q61] 移动平均
来源：http://hz.daria6918.cn/gtygzxaakk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.tanke756.top/gtjxsoanrg.html

[Q62] 分组占比
来源：http://hz.ivvv.top/gtwjbvkars.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tanke756.top/gtnxgbrruj.html

[Q63] 开启事务
来源：http://hz.gzhubu.top/gtdwlgdcgs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zdqjudy.top/gtzrqoczxj.html

[Q64] 提交事务
来源：http://hz.shanyushiyangtech.top/gttdnpcobt.html

COMMIT;
来源：http://hz.jinqigfzy.top/gthfopesno.html

[Q65] 回滚事务
来源：http://hz.hnxiangtu.top/gtwtnhgdmh.html

ROLLBACK;
来源：http://hz.daria6918.cn/gtphaqbydu.html

[Q66] 行锁查询
来源：http://hz.nanxuanxn.top/gtlmbmhdzi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hongshengwenyu.top/gttizoadhb.html

[Q67] 设置隔离级别
来源：http://hz.cashguo.top/gtbbrxidvi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ydzc1.top/gtrgayuydh.html

[Q68] 保存点
来源：http://hz.zdqjudy.top/gtfeanbksr.html

SAVEPOINT sp1;
来源：http://hz.tanke756.top/gtnsgizjdk.html

ROLLBACK TO sp1;
来源：http://hz.hammf.cn/gtdebajcgt.html

[Q69] 查看执行计划
来源：http://hz.ppjwa.cn/gtcizwfvbo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gaohongyu789.top/gtmeqeommj.html

[Q70] 更新统计信息
来源：http://hz.52xcode.cn/gtbcigbier.html

ANALYZE TABLE users;
来源：http://hz.yangfankeji.com/gtocagaxqt.html

[Q71] 查看建表语句
来源：http://hz.yuxming.cn/gtbmznsfia.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenzaomai.com/gtnwlkarrm.html

[Q72] 查看索引
来源：http://hz.cashguo.top/gtxqurbfia.html

SHOW INDEX FROM users;
来源：http://hz.9152youxi.cn/gtuoukhxti.html

[Q73] 查看表状态
来源：http://hz.wangdashe.top/gtvkutaocc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yangfankeji.com/gtqymdvayp.html

[Q74] 强制使用索引
来源：http://hz.shanyushiyangtech.top/gtgdjhvvkg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigfzy.top/gtycupvgdd.html

[Q75] 日期格式化
来源：http://hz.jqgfzy.top/gtwthajiww.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hfpthk.cn/gtrloiymug.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinqigfzy.top/gtgkgfndlp.html

[Q76] 按天统计
来源：http://hz.shanyushiyangtech.top/gtbtrbpclf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.dashuyun.cn/gtjweoufdh.html

[Q77] 时间加减
来源：http://hz.nwbrower.top/gtsrvwdoeg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinghuilouyu.cn/gtkzcngmul.html

[Q78] 当前时间
来源：http://hz.zhixingplan.top/gthktrirde.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.snrcjt.cn/gtmsodzaet.html

[Q79] 字符串拼接
来源：http://hz.ybcxt.top/gtkbbipuvq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xylfe.cn/gtvwvtfgqm.html

[Q80] 字符串截取
来源：http://hz.snrcjt.cn/gtjnkjezom.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jqgufenzy.top/gtphtjzhdj.html

[Q81] 字符串替换
来源：http://hz.sufxvd.cn/gtoadinypa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shanyushiyangtech.top/gtesoqqosp.html

[Q82] 字符长度与字节长度
来源：http://hz.jqgufenzy.top/gtcubzwucz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.chenlongwang.top/gtxqouzuko.html

[Q83] 大小写转换
来源：http://hz.c1oappe.top/gtdpdguxzd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.havefunace.top/gtctzugxts.html

[Q84] 去除首尾空格
来源：http://hz.shzxlz.cn/gtljypbstf.html

SELECT TRIM(name) FROM users;
来源：http://hz.birdmap.top/gttaywpuoe.html

[Q85] 数值取整
来源：http://hz.xingfuxueyuan.xyz/gtgbbiygsf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nanxinkj.top/gtjtkdnfay.html

[Q86] 读取 JSON 字段
来源：http://hz.316326.xyz/gtvdnrsbdl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.svipenyu.cn/gtepcwnaqg.html

[Q87] JSON 字段做条件
来源：http://hz.shuidangran.top/gtzqjtzjge.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.feifeiyinyue.top/gtcxytqskp.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhoulong.xyz/gtlwwkhhfx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cdnleiting.top/gtqdwlcoqz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.daria6918.cn/gtdanujjfv.html

[Q89] 判断表是否存在
来源：http://hz.yanxiufei.cn/gtzhqzjbsl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ydjk.org.cn/gtvngodjmu.html

[Q90] 生成序号列
来源：http://hz.fzhhl.top/gtgwhhnmqv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.feifeiyinyue.top/gthjembdmz.html

================================================================================
来源：http://hz.gotoacloud.top/gttbtzxtdl.html

R. Bash 专题
来源：http://hz.hysaishi.cn/gtkrzvudoo.html

================================================================================
来源：http://hz.andypj.xyz/gtlwxmbphi.html

[R01] shebang 与严格模式
来源：http://hz.jiagoushi.top/gtairynern.html

#!/usr/bin/env bash
来源：http://hz.yj202588.top/gtlgrbxcnq.html

set -euo pipefail
来源：http://hz.cdnleiting.top/gtgtlwrofb.html

[R02] 变量赋值与使用
来源：http://hz.cucudq.cn/gtaxvflgpw.html

name="Tom"; echo "$name"
来源：http://hz.hnqzz.top/gthuarruox.html

[R03] 只读变量
来源：http://hz.jiagoushi.top/gttcruwkwx.html

readonly PI=3.14
来源：http://hz.iojbl.cn/gthbdjukmz.html

[R04] 位置参数
来源：http://hz.zhijiandao.cn/gtnhjlthle.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.meibo888.top/gtnkwfpkzi.html

[R05] 参数默认值
来源：http://hz.jyoumei.cn/gtcgqkxbsi.html

name="${1:-default}"
来源：http://hz.hywenlv.cn/gtsczlwqoh.html

[R06] 判断命令是否存在
来源：http://hz.wangshuangyany.cn/gtqahedbne.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.c1oappe.top/gtdfpvpmex.html

[R07] if 判断文件
来源：http://hz.sxryk.cn/gtldwhudod.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenzaomai.com/gtvombgkxb.html

[R08] 数值比较
来源：http://hz.guannengcc.top/gtejencpfk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yuxming.cn/gtppggtjms.html

[R09] 字符串比较
来源：http://hz.hongshengwenyu.top/gtfyocipev.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhaomingkeji.xyz/gtxviphlir.html

[R10] 正则匹配
来源：http://hz.bjfxy.top/gttldurrdx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cqqwz.cn/gtxagusifc.html

[R11] case 多分支
来源：http://hz.gotoacloud.top/gtbspbjpkc.html

case "$1" in
来源：http://hz.yonumen.top/gtmjgosesv.html

start) echo "启动" ;;
来源：http://hz.cucudq.cn/gtafmukxtn.html

stop)  echo "停止" ;;
来源：http://hz.zhoulong.xyz/gtfjoeqsyr.html

*)     echo "未知命令" ;;
来源：http://hz.aizwys.cn/gtcrrbwmue.html

esac
来源：http://hz.jlsjyb.cn/gtaguqihsl.html

[R12] for 遍历文件
来源：http://hz.zycfv.cn/gtekodsowk.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xingfuxueyuan.xyz/gtwedaviqm.html

[R13] for 计数循环
来源：http://hz.gzhubu.top/gtrgqwnmjn.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jyoumei.cn/gtcqnydwfz.html

[R14] C 风格 for
来源：http://hz.xuanzx.com/gtkspazdxp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.daxiang520.top/gtpzgfhjfn.html

[R15] while 逐行读文件
来源：http://hz.jlsjyb.cn/gtxtzwzizn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinghuilouyu.cn/gtvuiwsbzu.html

[R16] until 等待条件
来源：http://hz.hnxiangtu.top/gthrcxnbnn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sysykeji.top/gtybpbkplf.html

[R17] 数组定义与取值
来源：http://hz.xuanzx.com/gtozkdvtam.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.52xcode.cn/gtohwrrueo.html

[R18] 遍历数组
来源：http://hz.hywenlv.cn/gtdeogncrk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangtech.top/gtamiwvzhb.html

[R19] 数组长度
来源：http://hz.zhiwuduotai.top/gtwgzwozex.html

echo "${#arr[@]}"
来源：http://hz.jinqigufen.top/gtesfohgod.html

[R20] 关联数组（字典）
来源：http://hz.xuetiantiany.cn/gtngntkbhs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.c1oappe.top/gtuhppskfz.html

[R21] 字符串长度
来源：http://hz.jyoumei.cn/gtdnxrajhw.html

echo "${#s}"
来源：http://hz.ehwqpu.com/gthyqzvrpp.html

[R22] 截取子串
来源：http://hz.kuanghao11.cn/gtxjpkvmkn.html

echo "${s:0:5}"
来源：http://hz.tanke756.top/gtsclxamya.html

[R23] 字符串替换
来源：http://hz.wangshuangyany.cn/gtdzvcocyx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinghuilouyu.cn/gttismbeds.html

[R24] 大小写转换
来源：http://hz.wangshuangyany.cn/gtjoauwazs.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sxryk.cn/gtyktjejty.html

[R25] 去后缀 / 去前缀
来源：http://hz.daxiang520.top/gtuollfnog.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.guowangkeji.top/gtosfnvwpb.html

[R26] 命令替换
来源：http://hz.haohaochexian.top/gtllpikmat.html

now=$(date +%F); echo "$now"
来源：http://hz.ydzc1.top/gtpiliorvh.html

[R27] 算术展开
来源：http://hz.svipenyu.cn/gtsvzdoeap.html

echo $((1 + 2 * 3))
来源：http://hz.cqqwz.cn/gthbpqpaly.html

[R28] 浮点运算
来源：http://hz.cashguo.top/gtbowhmbtq.html

echo "scale=2; 10/3" | bc
来源：http://hz.ehwqpu.com/gtrkyvawwh.html

[R29] 定义函数
来源：http://hz.9152youxi.cn/gtbtsmszlz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.havefunace.top/gtridpzzxm.html

[R30] 函数返回状态码
来源：http://hz.hongshengwenyu.top/gtakkcvpsv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhoulong.xyz/gttbxskvig.html

[R31] 局部变量
来源：http://hz.svipenyu.cn/gtlfgkbtmj.html

f() { local x=1; echo "$x"; }
来源：http://hz.jqgfzy.top/gtvhrbujyf.html

[R32] 参数个数校验
来源：http://hz.aizwys.cn/gtgfaejonc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hnqzz.top/gtspcxrfew.html

[R33] 捕获错误并提示行号
来源：http://hz.pengpengdd.cyou/gtwlfbunly.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hywenlv.cn/gtkiwfwsdo.html

[R34] 退出时清理
来源：http://hz.jqgfzy.top/gtecblefgv.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.haohaochexian.top/gtqohblvbu.html

[R35] 后台执行并等待
来源：http://hz.jqgfzy.top/gtknysioap.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.smart0.xyz/gterjovsia.html

[R36] 并发执行多个任务
来源：http://hz.hongshengwenyu.top/gtiinnfxoe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.bjfxy.top/gtajkjhjay.html

[R37] 把输出赋给变量
来源：http://hz.9152youxi.cn/gteavofqxf.html

files=$(ls -1)
来源：http://hz.dianchejie.cn/gtjcbtdojr.html

[R38] 管道串联
来源：http://hz.yanxiufei.cn/gtmfnmsoxm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cdnleiting.top/gtwkhstlcv.html

[R39] 重定向标准输出与错误
来源：http://hz.bjfxy.top/gtslldopon.html

cmd > out.log 2>&1
来源：http://hz.yvedp.cn/gtgbzqutek.html

[R40] 追加写日志
来源：http://hz.pengpengdd.cyou/gtwipybefb.html

echo "log" >> out.log
来源：http://hz.ydjk.org.cn/gtqmdrjxxq.html

[R41] 丢弃输出
来源：http://hz.yonumen.top/gtwejzteaj.html

cmd >/dev/null 2>&1
来源：http://hz.yuxming.cn/gttrjwvjgy.html

[R42] 输入重定向
来源：http://hz.jinyuanbaomall.cn/gtsyusvjxu.html

wc -l < a.txt
来源：http://hz.fengsongda.top/gtsdfnmdlp.html

[R43] 按名字查找文件
来源：http://hz.tian-w.cn/gthchmbehv.html

find . -name "*.log" -type f
来源：http://hz.ywan-chungtsiang.top/gtwnzjlwns.html

[R44] 按修改时间查找
来源：http://hz.0kj1m.cn/gtlcqijbuv.html

find . -mtime -7 -type f
来源：http://hz.ydjk.org.cn/gtmxvhcbuc.html

[R45] 批量删除
来源：http://hz.xziqi.cn/gtftctxaxx.html

find . -name "*.tmp" -delete
来源：http://hz.jyoumei.cn/gtqqrsqfvf.html

[R46] 递归替换文件内容
来源：http://hz.sufxvd.cn/gtwzvejvma.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xuetiantiany.cn/gtpwsblhdk.html

[R47] sed 单行替换
来源：http://hz.hysaishi.cn/gtrvxmxqjt.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xylfe.cn/gtuayyford.html

[R48] awk 取指定列
来源：http://hz.gotoacloud.top/gtuiuuorph.html

awk '{print $1, $3}' a.txt
来源：http://hz.xinyue.icu/gtyxibhuvy.html

[R49] awk 带条件
来源：http://hz.aizwys.cn/gtmredgvqm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhiwuduotai.top/gtdrjobqmp.html

[R50] awk 求和
来源：http://hz.fzhhl.top/gtastiqayu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj202588.top/gtruuvniof.html

[R51] 排序去重取前几
来源：http://hz.mhx1999.top/gtalfubrqh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cashguo.top/gtuhsyvzio.html

[R52] 统计行数
来源：http://hz.shzxlz.cn/gtirmplzng.html

wc -l a.txt
来源：http://hz.zycfv.cn/gtkmiygsli.html

[R53] 查看文件头与实时尾
来源：http://hz.jlsjyb.cn/gteivaejht.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhaomingkeji.xyz/gtnmtuiplr.html

[R54] 比较两个文件
来源：http://hz.aibaodan.cn/gtwowawdgk.html

diff a.txt b.txt
来源：http://hz.chenzaomai.com/gtdqwvanqn.html

[R55] 压缩与解压
来源：http://hz.nanxuanxn.top/gtsiqsmgig.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.mhx1999.top/gtalwfvlcd.html

[R56] 远程拷贝
来源：http://hz.jlsjyb.cn/gtkdvionik.html

scp file user@host:/path/
来源：http://hz.hnqzz.top/gtfeihlvse.html

[R57] 远程执行命令
来源：http://hz.nanxinkj.top/gtkqflcswu.html

ssh user@host 'uptime'
来源：http://hz.yueranfly.top/gtloogkebq.html

[R58] 下载文件
来源：http://hz.jyoumei.cn/gtafrkpiwn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zdqjudy.top/gtcxzrdkrn.html

[R59] 发 POST JSON
来源：http://hz.guannengcc.top/gtyjmjmkph.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.dashuyun.cn/gtzxplmxpy.html

[R60] 只看 HTTP 状态码
来源：http://hz.guannengcc.top/gtualpjzgf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yueranfly.top/gtoyiamwwl.html

[R61] 磁盘占用
来源：http://hz.redwolf501.top/gttygiyero.html

df -h;  du -sh *
来源：http://hz.daxiang520.top/gtcqceutnk.html

[R62] 找最占空间的文件
来源：http://hz.gzhubu.top/gtvqgjysot.html

du -ah . | sort -rh | head -10
来源：http://hz.xingfuxueyuan.xyz/gtwkbqnqxt.html

[R63] 内存与进程
来源：http://hz.jinyuanbaomall.cn/gtdgpotwpa.html

free -h;  ps aux | grep nginx
来源：http://hz.bjfxy.top/gtpcoruwvh.html

[R64] 结束进程
来源：http://hz.wangdashe.top/gtxpvmstjj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jyoumei.cn/gtujuplnsx.html

[R65] 查看端口占用
来源：http://hz.zhongyouzk.top/gtaabwgmff.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.iojbl.cn/gtlwmevkjb.html

[R66] 定时任务
来源：http://hz.hnxiangtu.top/gtxwqwpzwu.html

crontab -e;  crontab -l
来源：http://hz.redwolf501.top/gtjkihtgbq.html

[R67] 生成随机十六进制串
来源：http://hz.yonumen.top/gtcqrufckc.html

openssl rand -hex 16
来源：http://hz.gzhubu.top/gtxlcfjtol.html

[R68] 计算文件校验值
来源：http://hz.snrcjt.cn/gttjauntii.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cheryme.top/gtrnasjzlu.html

[R69] 生成随机密码
来源：http://hz.redwolf501.top/gtoxcnslgp.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinghuilouyu.cn/gtxdzdurtu.html

[R70] 时间戳与互转
来源：http://hz.yj20258.top/gtartcwcxa.html

date +%s;  date -d @1700000000
来源：http://hz.gzhubu.top/gtlxjwzmsu.html

[R71] 日期格式化
来源：http://hz.zycfv.cn/gtspibetue.html


<!-- 参考信息 -->