代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sysykeji.top/gtafuwraho.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj20258.top/gtdwxxxwlb.html

[Q13] 忽略重复插入
来源：http://hz.havefunace.top/gtrgchcxyy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhiwuduotai.top/gtllvwqwpc.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinqigfzy.top/gtnibsbmrg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yonumen.top/gtzykvuuab.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.meibo888.top/gtycblqrto.html

[Q15] 查询全部
来源：http://hz.zhixingplan.top/gtvjbujcjq.html

SELECT * FROM users;
来源：http://hz.chenjidiqi.icu/gtjigiypfo.html

[Q16] 查询指定列
来源：http://hz.cucudq.cn/gtvfontlmc.html

SELECT id, name FROM users;
来源：http://hz.xylfe.cn/gtstjkdtnj.html

[Q17] 条件查询
来源：http://hz.jinghuilouyu.cn/gtlvcwxzkk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hysaishi.cn/gtlzaxlxtp.html

[Q18] 模糊匹配
来源：http://hz.cqqwz.cn/gtljwkyvrz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yuxming.cn/gtcyrzjvru.html

[Q19] 范围查询
来源：http://hz.bjfxy.top/gtzawaxnzy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.redwolf501.top/gtspuluvqf.html

[Q20] IN 列表
来源：http://hz.jqgfzy.top/gtqeqlynxd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.aizwys.cn/gtzaephsfn.html

[Q21] 空值判断
来源：http://hz.hongshengwenyu.top/gtirzkwbjk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhijiandao.cn/gtyyjhmlxa.html

[Q22] 排序
来源：http://hz.xingfuxueyuan.xyz/gtvvhpybvq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tanke756.top/gtlihbthwd.html

[Q23] 分页
来源：http://hz.meibo888.top/gthqgsehjm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shanyushiyangtech.top/gtfgmrzyda.html

[Q24] 去重
来源：http://hz.pycfn.com/gtgenqstwj.html

SELECT DISTINCT city FROM users;
来源：http://hz.shzxlz.cn/gtncitswln.html

[Q25] 只取前 N 条
来源：http://hz.sxryk.cn/gtopialand.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.meibo888.top/gtfpolyevc.html

[Q26] 计数
来源：http://hz.feifeiyinyue.top/gthvipdjcq.html

SELECT COUNT(*) FROM users;
来源：http://hz.zdqjudy.top/gtzktmcozt.html

[Q27] 条件计数
来源：http://hz.jianghu66.top/gtzsnxdtgn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.andypj.xyz/gtmtnekopm.html

[Q28] 求和与平均
来源：http://hz.jiagoushi.top/gtgasdbbak.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.meibo888.top/gtdpxweglp.html

[Q29] 最大最小值
来源：http://hz.haohaochexian.top/gtzlvhgwae.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.nanxuanxn.top/gttbqkewzp.html

[Q30] 分组统计
来源：http://hz.sufxvd.cn/gtjvolkqqj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.haohaochexian.top/gtmyqequvt.html

[Q31] 分组后过滤
来源：http://hz.jiagoushi.top/gtobsayimk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.mhx1999.top/gtfkefvkpd.html

[Q32] 分组拼接字符串
来源：http://hz.dianchejie.cn/gtehlxuflq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtwtrlxfdi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ydzc1.top/gthpsiewbe.html

[Q33] 多列分组
来源：http://hz.ywan-chungtsiang.top/gtpfgqonmd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gaohongyu789.top/gtybffizab.html

[Q34] 每组取第一条
来源：http://hz.hammf.cn/gtzsfunoup.html

SELECT * FROM (
来源：http://hz.xingfuxueyuan.xyz/gtgeidltoc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.svipenyu.cn/gtiewxrhqq.html

) t WHERE rn = 1;
来源：http://hz.yuanzhike.top/gtyhnntwjg.html

[Q35] 内连接
来源：http://hz.hysaishi.cn/gtortzapzv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhijiandao.cn/gtbebcquly.html

[Q36] 左连接
来源：http://hz.pengpengdd.cyou/gtfxnztuua.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ybcxt.top/gtfwubjwig.html

[Q37] 右连接
来源：http://hz.hnxiangtu.top/gtovvynhez.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jqgufenzy.top/gtzhppicmn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jqgufenzy.top/gtzqtmeffd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.aibaodan.cn/gtdxijunza.html

[Q39] 自连接（查上下级）
来源：http://hz.jinghuilouyu.cn/gtxkuovubb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinghuilouyu.cn/gtztyjwjev.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.vqdsnc.cn/gtfnwvjscu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cqqwz.cn/gtxblxmdnf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yangfankeji.com/gtuavkosvl.html

[Q41] 多表连接
来源：http://hz.xylfe.cn/gtjjlexgin.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nanxuanxn.top/gtoubgshyc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhijiandao.cn/gtrahmwleu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xuetiantiany.cn/gtudnwoezg.html

[Q42] 连接条件附加过滤
来源：http://hz.guowangkeji.top/gtkbcofrlo.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cdnleiting.top/gtmmtimvwf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.redwolf501.top/gtrbfquhtc.html

[Q43] 标量子查询
来源：http://hz.haohaochexian.top/gtagixovmn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yuxming.cn/gtmjklewvn.html

[Q44] IN 子查询
来源：http://hz.jqgufenzy.top/gttvoxgats.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cashguo.top/gtukjbhobc.html

[Q45] EXISTS 判断存在
来源：http://hz.bjfxy.top/gteraysfbm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hongshengwenyu.top/gtnqdybups.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinyuanbaomall.cn/gtvzmpcgac.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuanzx.com/gtiifulfcy.html

[Q47] 与平均值比较
来源：http://hz.nanxuanxn.top/gtrmmtnmox.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.dashuyun.cn/gtavwnubtc.html

[Q48] CTE 公用表表达式
来源：http://hz.sxryk.cn/gtrejcjcxx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.fzhhl.top/gtonctgmrm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cashguo.top/gtsbpjukbl.html

[Q49] 更新单行
来源：http://hz.fengsongda.top/gtupyfkyls.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.daxiang520.top/gtapirqibb.html

[Q50] 批量更新
来源：http://hz.haohaochexian.top/gtdldtwtvm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zycfv.cn/gtybfbtzud.html

[Q51] 用子查询更新
来源：http://hz.jlsjyb.cn/gtcmazaxmc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jiagoushi.top/gtctxkhbqz.html

[Q52] 删除指定行
来源：http://hz.shanyushiyangtech.top/gtembwoecv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ydzc1.top/gtuggkshrl.html

[Q53] 按条件删除
来源：http://hz.hfpthk.cn/gtcmxvkmkh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.mhx1999.top/gtfahhjlsh.html

[Q54] 清空表
来源：http://hz.ydzc1.top/gtbozjqapq.html

TRUNCATE TABLE logs;
来源：http://hz.yj20258888.top/gtsqfmsaxm.html

[Q55] 排名（并列占位）
来源：http://hz.sweek.top/gtannswvla.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shangyingyoupin.top/gtfrjjcfgs.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhoulong.xyz/gtvymcfkoz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.guowangkeji.top/gtupanhffn.html

[Q57] 行号
来源：http://hz.svipenyu.cn/gtapwtqdts.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hywenlv.cn/gtjfeqngas.html

[Q58] 累计求和
来源：http://hz.fzhhl.top/gtvaizskmy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yuanzhike.top/gtzkhnjyht.html

[Q59] 分组内累计
来源：http://hz.zhaomingkeji.xyz/gtwermevvb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sufxvd.cn/gtykdbpbii.html

[Q60] 取上一行 / 下一行
来源：http://hz.guowangkeji.top/gtflbuiygp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhaomingkeji.xyz/gtubpuwnyg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinghuilouyu.cn/gtkpozyamw.html

[Q61] 移动平均
来源：http://hz.xuanzx.com/gtrdwhlmzi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenjidiqi.icu/gtuxwjxrzp.html

[Q62] 分组占比
来源：http://hz.jianghu66.top/gtjqpscoui.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.guannengcc.top/gtqdwutadm.html

[Q63] 开启事务
来源：http://hz.kuanghao11.cn/gtdyvhajwd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tianlin.xyz/gtyuwfxqji.html

[Q64] 提交事务
来源：http://hz.jinqigfzy.top/gtzzrjdvyl.html

COMMIT;
来源：http://hz.xingfuxueyuan.xyz/gtxevlrwcs.html

[Q65] 回滚事务
来源：http://hz.vqdsnc.cn/gtfhzjhuoe.html

ROLLBACK;
来源：http://hz.9152youxi.cn/gtmlzmmnwo.html

[Q66] 行锁查询
来源：http://hz.fengsongda.top/gtbacunefz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xuetiantiany.cn/gtslpiosdn.html

[Q67] 设置隔离级别
来源：http://hz.sweek.top/gtepsrfoqn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ywan-chungtsiang.top/gtvtqilter.html

[Q68] 保存点
来源：http://hz.guannengcc.top/gtdayozbfa.html

SAVEPOINT sp1;
来源：http://hz.havefunace.top/gtwonavznz.html

ROLLBACK TO sp1;
来源：http://hz.vqdsnc.cn/gtaekftuda.html

[Q69] 查看执行计划
来源：http://hz.feifeiyinyue.top/gtvetfibcy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhiwuduotai.top/gtokycnytd.html

[Q70] 更新统计信息
来源：http://hz.jqgufenzy.top/gtuiqyjxzn.html

ANALYZE TABLE users;
来源：http://hz.wangshuangyany.cn/gtgymotief.html

[Q71] 查看建表语句
来源：http://hz.jyoumei.cn/gtfzfedgag.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.vqdsnc.cn/gtwddqfyuy.html

[Q72] 查看索引
来源：http://hz.haohaochexian.top/gtawslfjdh.html

SHOW INDEX FROM users;
来源：http://hz.ydjk.org.cn/gtyhmumice.html

[Q73] 查看表状态
来源：http://hz.shangyingyoupin.top/gtjycdgyuf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhongyouzk.top/gtvpieadzv.html

[Q74] 强制使用索引
来源：http://hz.hammf.cn/gtxyjrxydo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zycfv.cn/gtmaltzdvg.html

[Q75] 日期格式化
来源：http://hz.jlsjyb.cn/gtlaoykdsb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gogol.net.cn/gtxdtlmmxn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hnxiangtu.top/gtiwnqopwb.html

[Q76] 按天统计
来源：http://hz.shangyingyoupin.top/gtuhntvkfy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.kuanghao11.cn/gtydwpbmvf.html

[Q77] 时间加减
来源：http://hz.quarkkingdee.top/gtpmxgfzru.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gogol.net.cn/gthmwophov.html

[Q78] 当前时间
来源：http://hz.hysaishi.cn/gtztsrgera.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.mhx1999.top/gtmbktybux.html

[Q79] 字符串拼接
来源：http://hz.yangfankeji.com/gtvbokuycv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.gaohongyu789.top/gtteotnbur.html

[Q80] 字符串截取
来源：http://hz.shuidangran.top/gtmtzeqdyo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gzhubu.top/gtfegewwrl.html

[Q81] 字符串替换
来源：http://hz.gzhubu.top/gtuxgvgtpe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gaohongyu789.top/gttctvgcii.html

[Q82] 字符长度与字节长度
来源：http://hz.xuanzx.com/gtbyynpspy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hongshengwenyu.top/gtthkhwmdd.html

[Q83] 大小写转换
来源：http://hz.ppjwa.cn/gtntpgqooy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.dianchejie.cn/gtsjcdgwpn.html

[Q84] 去除首尾空格
来源：http://hz.sxryk.cn/gtvltcehgq.html

SELECT TRIM(name) FROM users;
来源：http://hz.quarkkingdee.top/gttpwdhdfm.html

[Q85] 数值取整
来源：http://hz.jlsjyb.cn/gtidzhpznr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hysaishi.cn/gtketkuyst.html

[Q86] 读取 JSON 字段
来源：http://hz.xingfuxueyuan.xyz/gtygqeqrwt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhengqikj.top/gtqlvuiaaw.html

[Q87] JSON 字段做条件
来源：http://hz.sysykeji.top/gtgkhaqjhk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.aizwys.cn/gtynzckrij.html

[Q88] 行转列（条件聚合）
来源：http://hz.xylfe.cn/gttuiwcwot.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.haohaochexian.top/gtveowoxmw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.daxiang520.top/gtiizicqcu.html

[Q89] 判断表是否存在
来源：http://hz.ppjwa.cn/gtokrrbemd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.guowangkeji.top/gtwrnczvgi.html

[Q90] 生成序号列
来源：http://hz.meibo888.top/gtoedlkyuw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shangyingyoupin.top/gtneeacpgg.html

================================================================================
来源：http://hz.hnqzz.top/gtxmtgrhkg.html

R. Bash 专题
来源：http://hz.guannengcc.top/gtsazhsxch.html

================================================================================
来源：http://hz.ehwqpu.com/gtdegeipvl.html

[R01] shebang 与严格模式
来源：http://hz.mhx1999.top/gtgducyxqi.html

#!/usr/bin/env bash
来源：http://hz.havefunace.top/gtefnndyoc.html

set -euo pipefail
来源：http://hz.yj20258.top/gteduixkmg.html

[R02] 变量赋值与使用
来源：http://hz.xuetiantiany.cn/gtlebhmice.html

name="Tom"; echo "$name"
来源：http://hz.xinyue.icu/gtbzyyxbvk.html

[R03] 只读变量
来源：http://hz.feifeiyinyue.top/gtayxkszls.html

readonly PI=3.14
来源：http://hz.yongpay.top/gtarxhuatc.html

[R04] 位置参数
来源：http://hz.xuanzx.com/gtdbxgrorj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gaohongyu789.top/gtnemtbcet.html

[R05] 参数默认值
来源：http://hz.haohaochexian.top/gtnvmxaiqv.html

name="${1:-default}"
来源：http://hz.gogol.net.cn/gtdolpqqdk.html

[R06] 判断命令是否存在
来源：http://hz.0kj1m.cn/gtfcgxlbgf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.haohaochexian.top/gtglrekomj.html

[R07] if 判断文件
来源：http://hz.xuetiantiany.cn/gtvvhxyupo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.pengpengdd.cyou/gtcnnqnppu.html

[R08] 数值比较
来源：http://hz.yongpay.top/gtfywcqbfm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhiwuduotai.top/gtjhsmzban.html

[R09] 字符串比较
来源：http://hz.ybcxt.top/gtqhznuoas.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.haohaochexian.top/gtwqmvpqzn.html

[R10] 正则匹配
来源：http://hz.jqgfzy.top/gtblbfqzbn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.smart0.xyz/gtotxezxtj.html

[R11] case 多分支
来源：http://hz.xziqi.cn/gtoucaivda.html

case "$1" in
来源：http://hz.yuanzhike.top/gtzlzzqwca.html

start) echo "启动" ;;
来源：http://hz.gogol.net.cn/gtbgvwkawb.html

stop)  echo "停止" ;;
来源：http://hz.xingfuxueyuan.xyz/gtmxbmuwao.html

*)     echo "未知命令" ;;
来源：http://hz.316326.xyz/gtrvamvwcw.html

esac
来源：http://hz.xinyue.icu/gtvtgmrfav.html

[R12] for 遍历文件
来源：http://hz.jqgfzy.top/gtioyunpck.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hnxiangtu.top/gtqbbtsdmr.html

[R13] for 计数循环
来源：http://hz.yvedp.cn/gtgqshkupg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.bjfxy.top/gtfdhcdenf.html

[R14] C 风格 for
来源：http://hz.mhx1999.top/gtdveykgud.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zdqjudy.top/gtgnjomsvw.html

[R15] while 逐行读文件
来源：http://hz.jqgufenzy.top/gtdqdehpff.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhixingplan.top/gtqphzcged.html

[R16] until 等待条件
来源：http://hz.wangshuangyany.cn/gtlzcnstgc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yanxiufei.cn/gtvhqnjdgu.html

[R17] 数组定义与取值
来源：http://hz.zhengqikj.top/gtjagnlwsb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhaomingkeji.xyz/gtxlssmrpa.html

[R18] 遍历数组
来源：http://hz.guowangkeji.top/gtrvdhjnsx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jyoumei.cn/gtacezurln.html

[R19] 数组长度
来源：http://hz.yj20258888.top/gtjpofdwiw.html

echo "${#arr[@]}"
来源：http://hz.yuxming.cn/gtybnbmzdm.html

[R20] 关联数组（字典）
来源：http://hz.9152youxi.cn/gtnatmfria.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.9152youxi.cn/gtkbuhpooq.html

[R21] 字符串长度
来源：http://hz.sysykeji.top/gtupdbkjsb.html

echo "${#s}"
来源：http://hz.sufxvd.cn/gtuxlzyeth.html

[R22] 截取子串
来源：http://hz.birdmap.top/gtdrlcuyfb.html

echo "${s:0:5}"
来源：http://hz.svipenyu.cn/gtkslwsksj.html

[R23] 字符串替换
来源：http://hz.52xcode.cn/gtlwwtfnjz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.chenzaomai.com/gtdikjlkkc.html

[R24] 大小写转换
来源：http://hz.sufxvd.cn/gtmvcgrzcn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.meibo888.top/gtidnpxryo.html

[R25] 去后缀 / 去前缀
来源：http://hz.chenjidiqi.icu/gtlfblvenv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ywan-chungtsiang.top/gtyehjkfdp.html

[R26] 命令替换
来源：http://hz.c1oappe.top/gtyprycrha.html

now=$(date +%F); echo "$now"
来源：http://hz.9152youxi.cn/gtgwgkdodz.html

[R27] 算术展开
来源：http://hz.jinyuanbaomall.cn/gtxbjtjuuy.html

echo $((1 + 2 * 3))
来源：http://hz.vqdsnc.cn/gtxjjbmfkj.html

[R28] 浮点运算
来源：http://hz.jlsjyb.cn/gtupyxxjxe.html

echo "scale=2; 10/3" | bc
来源：http://hz.yueranfly.top/gtsmivjhtn.html

[R29] 定义函数
来源：http://hz.quarkkingdee.top/gtybxudjll.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinghuilouyu.cn/gtzieppoyn.html

[R30] 函数返回状态码
来源：http://hz.vqdsnc.cn/gtnmfxnbmn.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jqgufenzy.top/gtgjbagnwl.html

[R31] 局部变量
来源：http://hz.sysykeji.top/gtwdpcxjpo.html

f() { local x=1; echo "$x"; }
来源：http://hz.aibaodan.cn/gtndonokja.html

[R32] 参数个数校验
来源：http://hz.chenlongwang.top/gtyqwaiuyp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxuanxn.top/gtcatutvud.html

[R33] 捕获错误并提示行号
来源：http://hz.daxiang520.top/gtolmuxbdg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sxryk.cn/gtexjreuvt.html

[R34] 退出时清理
来源：http://hz.shangyingyoupin.top/gtzhvipxel.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinyuanbaomall.cn/gtfsofvton.html

[R35] 后台执行并等待
来源：http://hz.hammf.cn/gtbrgthoyw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sufxvd.cn/gtqqdiqtsj.html

[R36] 并发执行多个任务
来源：http://hz.ydjk.org.cn/gtmfffhqhk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shanyushiyangtech.top/gtroibnays.html

[R37] 把输出赋给变量
来源：http://hz.yj202588.top/gtdrtsjsus.html

files=$(ls -1)
来源：http://hz.feifeiyinyue.top/gtvjvmmcjw.html

[R38] 管道串联
来源：http://hz.ybcxt.top/gtlzcouxdx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ehwqpu.com/gtskcgaxtc.html

[R39] 重定向标准输出与错误
来源：http://hz.sysykeji.top/gtdggnfqmy.html

cmd > out.log 2>&1
来源：http://hz.xinyue.icu/gtvghhgorw.html

[R40] 追加写日志
来源：http://hz.shangyingyoupin.top/gtfcdchncv.html

echo "log" >> out.log
来源：http://hz.dashuyun.cn/gtzgwlfxzn.html

[R41] 丢弃输出
来源：http://hz.iojbl.cn/gtjslvkoik.html

cmd >/dev/null 2>&1
来源：http://hz.zdqjudy.top/gtjupddlta.html

[R42] 输入重定向
来源：http://hz.pycfn.com/gthoycgefn.html

wc -l < a.txt
来源：http://hz.guowangkeji.top/gtexrjecig.html

[R43] 按名字查找文件
来源：http://hz.hysaishi.cn/gtfnjnkdha.html

find . -name "*.log" -type f
来源：http://hz.ybcxt.top/gteasjbmcj.html

[R44] 按修改时间查找
来源：http://hz.gzhubu.top/gtjriuqvxy.html

find . -mtime -7 -type f
来源：http://hz.tanke756.top/gtibdgarls.html

[R45] 批量删除
来源：http://hz.guowangkeji.top/gtnnhpwulr.html

find . -name "*.tmp" -delete
来源：http://hz.svipenyu.cn/gtqwruoswk.html

[R46] 递归替换文件内容
来源：http://hz.pengpengdd.cyou/gtjahpmqei.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhiwuduotai.top/gtuhnazljv.html

[R47] sed 单行替换
来源：http://hz.shuidangran.top/gtunwkqxtl.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xinyue.icu/gttlvrdimo.html

[R48] awk 取指定列
来源：http://hz.cucudq.cn/gtzvhsbvpc.html

awk '{print $1, $3}' a.txt
来源：http://hz.gogol.net.cn/gtvftencql.html

[R49] awk 带条件
来源：http://hz.iojbl.cn/gtkntztrmb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jlsjyb.cn/gtejnjkekn.html

[R50] awk 求和
来源：http://hz.sysykeji.top/gtvskzbyus.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.vqdsnc.cn/gtagrpctzm.html

[R51] 排序去重取前几
来源：http://hz.hongshengwenyu.top/gtrchkhwgc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydzc1.top/gtspvgulgp.html

[R52] 统计行数
来源：http://hz.cashguo.top/gtmjnwvmvf.html

wc -l a.txt
来源：http://hz.cucudq.cn/gtoizdvtzl.html

[R53] 查看文件头与实时尾
来源：http://hz.quarkkingdee.top/gttaxykwnv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.pengpengdd.cyou/gtkbkdumlx.html

[R54] 比较两个文件
来源：http://hz.jiagoushi.top/gtxaerkgyh.html

diff a.txt b.txt
来源：http://hz.iojbl.cn/gtceuepmnf.html

[R55] 压缩与解压
来源：http://hz.meibo888.top/gtefggxfzf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shanyushiyangkeji.top/gtrvqawbjt.html

[R56] 远程拷贝
来源：http://hz.jiagoushi.top/gtjtzhlbtr.html

scp file user@host:/path/
来源：http://hz.tian-w.cn/gtwzawautn.html

[R57] 远程执行命令
来源：http://hz.redwolf501.top/gtkugdvwfa.html

ssh user@host 'uptime'
来源：http://hz.yuanzhike.top/gthzphxujx.html

[R58] 下载文件
来源：http://hz.sweek.top/gtmbzxqzrp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hnxiangtu.top/gtskthnqav.html

[R59] 发 POST JSON
来源：http://hz.chenzaomai.com/gtxlmayktd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hnqzz.top/gttjifxzot.html

[R60] 只看 HTTP 状态码
来源：http://hz.xuanzx.com/gtnsqtbuha.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tanke756.top/gtqjqxdciq.html

[R61] 磁盘占用
来源：http://hz.yj20258888.top/gtugdntpum.html


<!-- 参考信息 -->