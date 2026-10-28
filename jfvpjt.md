代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://hz.aibaodan.cn/gtervqkszx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cashguo.top/gtynbmhmfe.html

[Q13] 忽略重复插入
来源：http://hz.mhx1999.top/gtbqrjeirm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.pengpengdd.cyou/gtdyhbrvzb.html

[Q14] 存在则更新（upsert）
来源：http://hz.hywenlv.cn/gtyxpinlfg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ivvv.top/gtjtgdgfox.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xinyue.icu/gtkunfmdvg.html

[Q15] 查询全部
来源：http://hz.guowangkeji.top/gtqkkqerry.html

SELECT * FROM users;
来源：http://hz.nanxuanxn.top/gtgztsuhoh.html

[Q16] 查询指定列
来源：http://hz.quarkkingdee.top/gtliwgxdsc.html

SELECT id, name FROM users;
来源：http://hz.chenjidiqi.icu/gtekyvjcfu.html

[Q17] 条件查询
来源：http://hz.daria6918.cn/gtxuoujcdv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cdnleiting.top/gtsbffjsbr.html

[Q18] 模糊匹配
来源：http://hz.daxiang520.top/gtbqvyumjl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ywan-chungtsiang.top/gtffbjegxm.html

[Q19] 范围查询
来源：http://hz.hywenlv.cn/gtxoufglpv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ppjwa.cn/gtsyrmwsyr.html

[Q20] IN 列表
来源：http://hz.chenjidiqi.icu/gtvfslhzdx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ivvv.top/gtvtejputr.html

[Q21] 空值判断
来源：http://hz.ivvv.top/gtqnciotgw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shuidangran.top/gtdfjbkcui.html

[Q22] 排序
来源：http://hz.xylfe.cn/gtzulysutz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hammf.cn/gtyqbrrmzg.html

[Q23] 分页
来源：http://hz.cashguo.top/gtxyvfyavk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ppjwa.cn/gtcevscbsw.html

[Q24] 去重
来源：http://hz.zhaomingkeji.xyz/gtzjqdvols.html

SELECT DISTINCT city FROM users;
来源：http://hz.fzhhl.top/gtkddxbskh.html

[Q25] 只取前 N 条
来源：http://hz.sweek.top/gtzocbuhxy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hammf.cn/gtupspjnif.html

[Q26] 计数
来源：http://hz.yj202588.top/gtjnruuzhi.html

SELECT COUNT(*) FROM users;
来源：http://hz.aizwys.cn/gtgktciegl.html

[Q27] 条件计数
来源：http://hz.wangdashe.top/gtokzwjarc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ydjk.org.cn/gtouinwrmq.html

[Q28] 求和与平均
来源：http://hz.havefunace.top/gtpzwbklqy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.nanxinkj.top/gtnvyttexm.html

[Q29] 最大最小值
来源：http://hz.birdmap.top/gtlcjajmzo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zdqjudy.top/gtcdwgajrf.html

[Q30] 分组统计
来源：http://hz.ehwqpu.com/gtwkdqemvn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.smart0.xyz/gtdytshkpt.html

[Q31] 分组后过滤
来源：http://hz.zhijiandao.cn/gtdbonyafr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cashguo.top/gtdmcvwdxa.html

[Q32] 分组拼接字符串
来源：http://hz.ehwqpu.com/gtrtpljipc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtudyttjdb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhoulong.xyz/gtmorlomay.html

[Q33] 多列分组
来源：http://hz.daxiang520.top/gtmtvwwvrj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.nanxuanxn.top/gtgdscfayk.html

[Q34] 每组取第一条
来源：http://hz.shuidangran.top/gtxjcljaau.html

SELECT * FROM (
来源：http://hz.jiagoushi.top/gtxyimqlst.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hysaishi.cn/gtrckpvtpv.html

) t WHERE rn = 1;
来源：http://hz.jlsjyb.cn/gtuulejlup.html

[Q35] 内连接
来源：http://hz.sufxvd.cn/gtpardcrlx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jlsjyb.cn/gtjbzcxsrs.html

[Q36] 左连接
来源：http://hz.xinyue.icu/gtseclhnfb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhijiandao.cn/gtuzaunyfn.html

[Q37] 右连接
来源：http://hz.havefunace.top/gtkpdyjwem.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.guannengcc.top/gtwsptqtwk.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yvedp.cn/gtxudemxrm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hysaishi.cn/gtzadaeifr.html

[Q39] 自连接（查上下级）
来源：http://hz.aizwys.cn/gtejqxqbbi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shzxlz.cn/gtkwcyrpne.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yangfankeji.com/gtwrmkcwml.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xziqi.cn/gtgiuelnuy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hnxiangtu.top/gtspoougwo.html

[Q41] 多表连接
来源：http://hz.ivvv.top/gtzukgnwqm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ywan-chungtsiang.top/gtfavkfdty.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shanyushiyangkeji.top/gtiwviwlmf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.snrcjt.cn/gtaglohenj.html

[Q42] 连接条件附加过滤
来源：http://hz.quarkkingdee.top/gtlkqdfviw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ydjk.org.cn/gtsdktbsld.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangshuangyany.cn/gtmxfwmzrb.html

[Q43] 标量子查询
来源：http://hz.svipenyu.cn/gtmzuexrro.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.c1oappe.top/gtsvpjastd.html

[Q44] IN 子查询
来源：http://hz.andypj.xyz/gtdjhptgkd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.svipenyu.cn/gtbbzyphfv.html

[Q45] EXISTS 判断存在
来源：http://hz.ydjk.org.cn/gtoyiycvan.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aizwys.cn/gtyipwvmco.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.316326.xyz/gtjuzmfrrg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nwbrower.top/gtnjpxzsmj.html

[Q47] 与平均值比较
来源：http://hz.gotoacloud.top/gtbpiwcjsj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinyuanbaomall.cn/gtyyyegiin.html

[Q48] CTE 公用表表达式
来源：http://hz.guannengcc.top/gtbhvooddj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhengqikj.top/gtwsoktczw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.dianchejie.cn/gtlxoikrmm.html

[Q49] 更新单行
来源：http://hz.svipenyu.cn/gtchfkavyx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gaohongyu789.top/gtpwivqqnf.html

[Q50] 批量更新
来源：http://hz.pycfn.com/gtjvsabred.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinghuilouyu.cn/gtlzudbaqs.html

[Q51] 用子查询更新
来源：http://hz.birdmap.top/gtzfjvunvz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ehwqpu.com/gtrmhywzbk.html

[Q52] 删除指定行
来源：http://hz.zhoulong.xyz/gtjtfbwnha.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hysaishi.cn/gtcajwthuu.html

[Q53] 按条件删除
来源：http://hz.hfpthk.cn/gtwylzhnbb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.fengsongda.top/gtrxpkaxph.html

[Q54] 清空表
来源：http://hz.bjfxy.top/gtmonsdzll.html

TRUNCATE TABLE logs;
来源：http://hz.quarkkingdee.top/gtulbqfbne.html

[Q55] 排名（并列占位）
来源：http://hz.cqqwz.cn/gtkryygnza.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.wangdashe.top/gtlmsajqvw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinqigfzy.top/gtgjeyiioe.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.chenjidiqi.icu/gtzjtctodi.html

[Q57] 行号
来源：http://hz.yj20258.top/gtnhgnmytd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.kuanghao11.cn/gtlbkutkvo.html

[Q58] 累计求和
来源：http://hz.xuanzx.com/gtbsoryxpi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shangyingyoupin.top/gtsqdhkuno.html

[Q59] 分组内累计
来源：http://hz.svipenyu.cn/gtmxkhyqkx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.316326.xyz/gthphscjiz.html

[Q60] 取上一行 / 下一行
来源：http://hz.mhx1999.top/gtqdncjiqa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhengqikj.top/gtnxrldiyn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhijiandao.cn/gtojfjgvmc.html

[Q61] 移动平均
来源：http://hz.yvedp.cn/gtdtxshehc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xylfe.cn/gtesteggey.html

[Q62] 分组占比
来源：http://hz.ybcxt.top/gtfftkhoqz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gtwkrgcnhq.html

[Q63] 开启事务
来源：http://hz.yuanzhike.top/gtvsscikrf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.fengsongda.top/gtmwpkyisf.html

[Q64] 提交事务
来源：http://hz.yanxiufei.cn/gtnuprsgpy.html

COMMIT;
来源：http://hz.hongshengwenyu.top/gtnklaxhqv.html

[Q65] 回滚事务
来源：http://hz.gaohongyu789.top/gtyfyvyqos.html

ROLLBACK;
来源：http://hz.gaohongyu789.top/gtdldkwtro.html

[Q66] 行锁查询
来源：http://hz.zhiwuduotai.top/gtqiglhtuk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gaohongyu789.top/gtbegxgviu.html

[Q67] 设置隔离级别
来源：http://hz.zhiwuduotai.top/gtkviwqbpa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xuanzx.com/gtjsdbvgpx.html

[Q68] 保存点
来源：http://hz.shzxlz.cn/gtvfehqecl.html

SAVEPOINT sp1;
来源：http://hz.bjfxy.top/gthpqfeidg.html

ROLLBACK TO sp1;
来源：http://hz.tanke756.top/gtxlepborr.html

[Q69] 查看执行计划
来源：http://hz.jqgfzy.top/gtiglmilux.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.smart0.xyz/gtfrtarpsl.html

[Q70] 更新统计信息
来源：http://hz.mhx1999.top/gthujjzgzq.html

ANALYZE TABLE users;
来源：http://hz.jinqigfzy.top/gtyomreakv.html

[Q71] 查看建表语句
来源：http://hz.hfpthk.cn/gtenyyjcuj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hnqzz.top/gtpvodrmbl.html

[Q72] 查看索引
来源：http://hz.316326.xyz/gtehcspevj.html

SHOW INDEX FROM users;
来源：http://hz.nwbrower.top/gtpegeasbv.html

[Q73] 查看表状态
来源：http://hz.xingfuxueyuan.xyz/gtsvwghcox.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.vqdsnc.cn/gtdaqaxaie.html

[Q74] 强制使用索引
来源：http://hz.pycfn.com/gtdefflvrf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.feifeiyinyue.top/gtaxyebhkl.html

[Q75] 日期格式化
来源：http://hz.zhijiandao.cn/gttfybzjef.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ivvv.top/gtymcdxxib.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zdqjudy.top/gtgszvmcvk.html

[Q76] 按天统计
来源：http://hz.316326.xyz/gtoxplcvnm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tian-w.cn/gtbhalgbpo.html

[Q77] 时间加减
来源：http://hz.yueranfly.top/gtcrvdndgg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinqigfzy.top/gtbyopyqdx.html

[Q78] 当前时间
来源：http://hz.52xcode.cn/gtkkavmrqn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.chenlongwang.top/gtfofukqlk.html

[Q79] 字符串拼接
来源：http://hz.yangfankeji.com/gtddqqclik.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yangfankeji.com/gtmiypjrmb.html

[Q80] 字符串截取
来源：http://hz.redwolf501.top/gtdgikctgo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hnqzz.top/gtyccgqmnv.html

[Q81] 字符串替换
来源：http://hz.xylfe.cn/gtxbidfabc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hysaishi.cn/gtcxtjqkjr.html

[Q82] 字符长度与字节长度
来源：http://hz.ydjk.org.cn/gtvwejwwrc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cheryme.top/gtpxquyarp.html

[Q83] 大小写转换
来源：http://hz.aizwys.cn/gtizppzrad.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinqigfzy.top/gtealpaabq.html

[Q84] 去除首尾空格
来源：http://hz.aizwys.cn/gtgemakkxw.html

SELECT TRIM(name) FROM users;
来源：http://hz.yangfankeji.com/gtqglelzbq.html

[Q85] 数值取整
来源：http://hz.xziqi.cn/gtmafubtrh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hywenlv.cn/gtbhklofvm.html

[Q86] 读取 JSON 字段
来源：http://hz.meibo888.top/gtzdzcyerp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cqqwz.cn/gtyfksuzud.html

[Q87] JSON 字段做条件
来源：http://hz.xuanzx.com/gtqgpmshyl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.bjfxy.top/gtzplalpjg.html

[Q88] 行转列（条件聚合）
来源：http://hz.cdnleiting.top/gtqjvljzkv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.snrcjt.cn/gtakwjdchm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.snrcjt.cn/gtavlxrwae.html

[Q89] 判断表是否存在
来源：http://hz.bjfxy.top/gtpzlqfaom.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.guowangkeji.top/gtqgxgiusz.html

[Q90] 生成序号列
来源：http://hz.ehwqpu.com/gttckugduj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.birdmap.top/gtpeuvfqil.html

================================================================================
来源：http://hz.yuxming.cn/gtwzfzszoq.html

R. Bash 专题
来源：http://hz.ydzc1.top/gthcqgfnrq.html

================================================================================
来源：http://hz.daria6918.cn/gtmrvizxun.html

[R01] shebang 与严格模式
来源：http://hz.hnxiangtu.top/gtioexuwru.html

#!/usr/bin/env bash
来源：http://hz.yangfankeji.com/gtnpoznsgo.html

set -euo pipefail
来源：http://hz.zhongyouzk.top/gtrupgxvps.html

[R02] 变量赋值与使用
来源：http://hz.havefunace.top/gtmtayuakz.html

name="Tom"; echo "$name"
来源：http://hz.c1oappe.top/gtufwfmtls.html

[R03] 只读变量
来源：http://hz.iojbl.cn/gtmttddtbd.html

readonly PI=3.14
来源：http://hz.ywan-chungtsiang.top/gtyeulbfhr.html

[R04] 位置参数
来源：http://hz.tian-w.cn/gtqvpfdomm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenzaomai.com/gtaafpvobe.html

[R05] 参数默认值
来源：http://hz.svipenyu.cn/gtnfylwcog.html

name="${1:-default}"
来源：http://hz.hnqzz.top/gtlznebqnf.html

[R06] 判断命令是否存在
来源：http://hz.jianghu66.top/gtyoxhrqet.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhixingplan.top/gtndkvcfhp.html

[R07] if 判断文件
来源：http://hz.zhengqikj.top/gtcskzxidn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinqigufen.top/gtfgnoazeb.html

[R08] 数值比较
来源：http://hz.fzhhl.top/gtpamjuxtt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.birdmap.top/gtlhltflsc.html

[R09] 字符串比较
来源：http://hz.xingfuxueyuan.xyz/gtnrzuxadk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hnxiangtu.top/gtfrmpzlhk.html

[R10] 正则匹配
来源：http://hz.xuanzx.com/gtpfgfxhxj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cheryme.top/gtfjvpbgra.html

[R11] case 多分支
来源：http://hz.sufxvd.cn/gtecpicjfy.html

case "$1" in
来源：http://hz.yj202588.top/gtauedunmc.html

start) echo "启动" ;;
来源：http://hz.yongpay.top/gthroqqmrc.html

stop)  echo "停止" ;;
来源：http://hz.shanyushiyangtech.top/gtivaivycm.html

*)     echo "未知命令" ;;
来源：http://hz.sufxvd.cn/gttbkfzeeo.html

esac
来源：http://hz.daxiang520.top/gtfyuiajmt.html

[R12] for 遍历文件
来源：http://hz.wangdashe.top/gtsdkwncjd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sysykeji.top/gtpsicruxp.html

[R13] for 计数循环
来源：http://hz.jinyuanbaomall.cn/gtmmzltveq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.pycfn.com/gtandeykxt.html

[R14] C 风格 for
来源：http://hz.hongshengwenyu.top/gtaftqnqqc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xziqi.cn/gtuujptycw.html

[R15] while 逐行读文件
来源：http://hz.jlsjyb.cn/gtecwfqjqb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhoulong.xyz/gtexpiyzkz.html

[R16] until 等待条件
来源：http://hz.tianlin.xyz/gttolzbcbm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.pengpengdd.cyou/gthfumrlvy.html

[R17] 数组定义与取值
来源：http://hz.hywenlv.cn/gtevkctgxh.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.iojbl.cn/gtuajjmlmx.html

[R18] 遍历数组
来源：http://hz.jyoumei.cn/gtprxfgjdp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhiwuduotai.top/gtwbzgmnep.html

[R19] 数组长度
来源：http://hz.daria6918.cn/gtnjlcskae.html

echo "${#arr[@]}"
来源：http://hz.sysykeji.top/gtpqulfxjn.html

[R20] 关联数组（字典）
来源：http://hz.zycfv.cn/gtgjmolpni.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ybcxt.top/gtcxhujhdk.html

[R21] 字符串长度
来源：http://hz.ppjwa.cn/gtnbvbbkak.html

echo "${#s}"
来源：http://hz.jinqigufen.top/gtfgnajgil.html

[R22] 截取子串
来源：http://hz.daxiang520.top/gtyaxqbqam.html

echo "${s:0:5}"
来源：http://hz.ywan-chungtsiang.top/gtlbxqqvnr.html

[R23] 字符串替换
来源：http://hz.yonumen.top/gtmqjtosfi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinghuilouyu.cn/gtwayzirqz.html

[R24] 大小写转换
来源：http://hz.feifeiyinyue.top/gtwiwkfuem.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jqgufenzy.top/gtljihmots.html

[R25] 去后缀 / 去前缀
来源：http://hz.mhx1999.top/gtjkyhvawr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ivvv.top/gtqjhwmilf.html

[R26] 命令替换
来源：http://hz.ydzc1.top/gtyhqbusjw.html

now=$(date +%F); echo "$now"
来源：http://hz.xuanzx.com/gtmggbufjy.html

[R27] 算术展开
来源：http://hz.sweek.top/gtwirulxbk.html

echo $((1 + 2 * 3))
来源：http://hz.ppjwa.cn/gtegcrhcmg.html

[R28] 浮点运算
来源：http://hz.yueranfly.top/gtfdymlrzm.html

echo "scale=2; 10/3" | bc
来源：http://hz.gogol.net.cn/gtnooyptyd.html

[R29] 定义函数
来源：http://hz.zhiwuduotai.top/gtyuyqinzt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.daria6918.cn/gtihyznpqk.html

[R30] 函数返回状态码
来源：http://hz.shzxlz.cn/gtglqrvibx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhaomingkeji.xyz/gtxjyuspsv.html

[R31] 局部变量
来源：http://hz.zdqjudy.top/gtknientcc.html

f() { local x=1; echo "$x"; }
来源：http://hz.hammf.cn/gtnjpuvziw.html

[R32] 参数个数校验
来源：http://hz.wangdashe.top/gtagmblbqg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinyuanbaomall.cn/gtmarppmpf.html

[R33] 捕获错误并提示行号
来源：http://hz.zhiwuduotai.top/gtpdfjvmgb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.0kj1m.cn/gthzyyamfd.html

[R34] 退出时清理
来源：http://hz.zhiwuduotai.top/gtnlvdewkn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.daria6918.cn/gtdxyeishi.html

[R35] 后台执行并等待
来源：http://hz.tian-w.cn/gtoqzrxjxb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.dianchejie.cn/gtaqzqiesl.html

[R36] 并发执行多个任务
来源：http://hz.svipenyu.cn/gtwfvxchfo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ydzc1.top/gtiqfvduew.html

[R37] 把输出赋给变量
来源：http://hz.gogol.net.cn/gtraltmxsu.html

files=$(ls -1)
来源：http://hz.svipenyu.cn/gtywnyiknv.html

[R38] 管道串联
来源：http://hz.jinqigfzy.top/gtzljlmhob.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yuanzhike.top/gtbmhdodam.html

[R39] 重定向标准输出与错误
来源：http://hz.snrcjt.cn/gtbtyjdywg.html

cmd > out.log 2>&1
来源：http://hz.snrcjt.cn/gtryoykvxu.html

[R40] 追加写日志
来源：http://hz.zhaomingkeji.xyz/gthhfdzeda.html

echo "log" >> out.log
来源：http://hz.316326.xyz/gtestmozgd.html

[R41] 丢弃输出
来源：http://hz.fzhhl.top/gtcptmrmiv.html

cmd >/dev/null 2>&1
来源：http://hz.zdqjudy.top/gtnamjojwf.html

[R42] 输入重定向
来源：http://hz.nanxinkj.top/gttflniprf.html

wc -l < a.txt
来源：http://hz.jinqigufen.top/gtudmedyec.html

[R43] 按名字查找文件
来源：http://hz.tian-w.cn/gtdujhucqb.html

find . -name "*.log" -type f
来源：http://hz.smart0.xyz/gtwwxtdjqe.html

[R44] 按修改时间查找
来源：http://hz.chenzaomai.com/gtvoljvqrp.html

find . -mtime -7 -type f
来源：http://hz.xuanzx.com/gtbzejtxyk.html

[R45] 批量删除
来源：http://hz.zhongyouzk.top/gtzkobifyf.html

find . -name "*.tmp" -delete
来源：http://hz.guannengcc.top/gtdjvqkctr.html

[R46] 递归替换文件内容
来源：http://hz.mhx1999.top/gtlbzdrrer.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhongyouzk.top/gtadoxogyu.html

[R47] sed 单行替换
来源：http://hz.dashuyun.cn/gthzojsqub.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jyoumei.cn/gtrgztceek.html

[R48] awk 取指定列
来源：http://hz.feifeiyinyue.top/gtydlijvqo.html

awk '{print $1, $3}' a.txt
来源：http://hz.pengpengdd.cyou/gtuyeeeajq.html

[R49] awk 带条件
来源：http://hz.tanke756.top/gtgjgnvtfi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ybcxt.top/gtgobxcmnb.html

[R50] awk 求和
来源：http://hz.yj20258.top/gtpkslvncl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhaomingkeji.xyz/gtxsvldqyh.html

[R51] 排序去重取前几
来源：http://hz.hnxiangtu.top/gtuhrrjrof.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.dianchejie.cn/gtcamgbpuw.html

[R52] 统计行数
来源：http://hz.yj20258.top/gtixyfvtsp.html

wc -l a.txt
来源：http://hz.yvedp.cn/gtoiltumog.html

[R53] 查看文件头与实时尾
来源：http://hz.wangdashe.top/gtzhtilvoz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xziqi.cn/gtilubrlbg.html

[R54] 比较两个文件
来源：http://hz.shuidangran.top/gtototbyey.html

diff a.txt b.txt
来源：http://hz.zhixingplan.top/gtuljcshse.html

[R55] 压缩与解压
来源：http://hz.zhijiandao.cn/gtognoscit.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yangfankeji.com/gtkjulrpiz.html

[R56] 远程拷贝
来源：http://hz.nanxinkj.top/gtajgyqcgo.html

scp file user@host:/path/
来源：http://hz.fengsongda.top/gtnfpqzilp.html

[R57] 远程执行命令
来源：http://hz.bjfxy.top/gtopcslaub.html

ssh user@host 'uptime'
来源：http://hz.sufxvd.cn/gttadorpuf.html

[R58] 下载文件
来源：http://hz.hysaishi.cn/gtetayvhhb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yongpay.top/gtinconpen.html

[R59] 发 POST JSON
来源：http://hz.jiagoushi.top/gticcxvrww.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hywenlv.cn/gtvnrsvmvv.html

[R60] 只看 HTTP 状态码
来源：http://hz.jyoumei.cn/gtocdorvhl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.52xcode.cn/gtllaaxwhp.html

[R61] 磁盘占用
来源：http://hz.dianchejie.cn/gtcmyjygev.html


<!-- 参考信息 -->