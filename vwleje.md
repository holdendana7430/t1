代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhongyouzk.top/gtissnohgl.html

[Q20] IN 列表
来源：http://hz.quarkkingdee.top/gtotydkhjw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gogol.net.cn/gtytyksleu.html

[Q21] 空值判断
来源：http://hz.yangfankeji.com/gtbqoywmlr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.fengsongda.top/gtjdcmqyob.html

[Q22] 排序
来源：http://hz.sufxvd.cn/gteaktlsva.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ydzc1.top/gtnqokibri.html

[Q23] 分页
来源：http://hz.fzhhl.top/gtavpkpagw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ydzc1.top/gtdmidjhzx.html

[Q24] 去重
来源：http://hz.bjfxy.top/gtgkwlifdd.html

SELECT DISTINCT city FROM users;
来源：http://hz.yonumen.top/gttxhhkwoz.html

[Q25] 只取前 N 条
来源：http://hz.sxryk.cn/gtdmnwqrxp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.dianchejie.cn/gtkjzagmjq.html

[Q26] 计数
来源：http://hz.redwolf501.top/gtlfiijrcv.html

SELECT COUNT(*) FROM users;
来源：http://hz.daxiang520.top/gtgvzqyvoa.html

[Q27] 条件计数
来源：http://hz.ydjk.org.cn/gtmvdsctyw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yuxming.cn/gtswkuaujd.html

[Q28] 求和与平均
来源：http://hz.chenjidiqi.icu/gtvohmzcmx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtaweuniuf.html

[Q29] 最大最小值
来源：http://hz.hywenlv.cn/gtoytfsscr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cheryme.top/gtsbxbtghr.html

[Q30] 分组统计
来源：http://hz.wangshuangyany.cn/gtjicetauw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.chenjidiqi.icu/gtqrcmxtxj.html

[Q31] 分组后过滤
来源：http://hz.svipenyu.cn/gtzvgbamel.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.guannengcc.top/gtgpsusake.html

[Q32] 分组拼接字符串
来源：http://hz.tian-w.cn/gtkyxeqmmd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.havefunace.top/gtgibbkavv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yuxming.cn/gtvjknmmpo.html

[Q33] 多列分组
来源：http://hz.meibo888.top/gtqxdndibs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.52xcode.cn/gtbiracaap.html

[Q34] 每组取第一条
来源：http://hz.gzhubu.top/gtmuebuttl.html

SELECT * FROM (
来源：http://hz.daria6918.cn/gtsdtieeas.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ybcxt.top/gtfzwwcavb.html

) t WHERE rn = 1;
来源：http://hz.0kj1m.cn/gtuhpxfdag.html

[Q35] 内连接
来源：http://hz.shanyushiyangkeji.top/gtopifpnlm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtllgsdaml.html

[Q36] 左连接
来源：http://hz.zhiwuduotai.top/gtkywzucec.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hfpthk.cn/gtarspgeqa.html

[Q37] 右连接
来源：http://hz.nanxinkj.top/gtetshxumk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinghuilouyu.cn/gtltfljmgs.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jiagoushi.top/gtdmpreaur.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ydzc1.top/gtuogfkbtm.html

[Q39] 自连接（查上下级）
来源：http://hz.fzhhl.top/gturujexjv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.meibo888.top/gtywteltnd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hywenlv.cn/gtsudafrdb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.kuanghao11.cn/gtmbjtugpw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yj20258.top/gtcovpqkpc.html

[Q41] 多表连接
来源：http://hz.zhiwuduotai.top/gtucnpfjfs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhoulong.xyz/gtwwmoyibn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shuidangran.top/gtkwirbjzw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shzxlz.cn/gtivckwdnq.html

[Q42] 连接条件附加过滤
来源：http://hz.birdmap.top/gtzrrzqzje.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jyoumei.cn/gtqbsybcgh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.dianchejie.cn/gtbsjqpobh.html

[Q43] 标量子查询
来源：http://hz.gaohongyu789.top/gtxmvazswo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhengqikj.top/gtcnchjwzy.html

[Q44] IN 子查询
来源：http://hz.sufxvd.cn/gtvrbeykul.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.nwbrower.top/gtuphyjiwf.html

[Q45] EXISTS 判断存在
来源：http://hz.cashguo.top/gtbvyktfsc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenzaomai.com/gtsouqessh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xingfuxueyuan.xyz/gtzbxcczpa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gtldahxdtj.html

[Q47] 与平均值比较
来源：http://hz.jiagoushi.top/gtjeazpmfd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.aibaodan.cn/gtydyeilyj.html

[Q48] CTE 公用表表达式
来源：http://hz.jinqigufen.top/gtppzqmslq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.sufxvd.cn/gtqwnbbzsf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.iojbl.cn/gtsrfxapro.html

[Q49] 更新单行
来源：http://hz.zhoulong.xyz/gtmrjjecjs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj202588.top/gtychsmrkm.html

[Q50] 批量更新
来源：http://hz.zhijiandao.cn/gtomzyrtae.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhengqikj.top/gtibualgom.html

[Q51] 用子查询更新
来源：http://hz.ydjk.org.cn/gttwexfupv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhongyouzk.top/gtlxmxlgxd.html

[Q52] 删除指定行
来源：http://hz.gogol.net.cn/gtnbsfizsy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhongyouzk.top/gtrubwcxys.html

[Q53] 按条件删除
来源：http://hz.zycfv.cn/gtsoqdqxha.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sxryk.cn/gtiuwnywcv.html

[Q54] 清空表
来源：http://hz.shanyushiyangkeji.top/gtwyyjrcpz.html

TRUNCATE TABLE logs;
来源：http://hz.sysykeji.top/gtkahkoswx.html

[Q55] 排名（并列占位）
来源：http://hz.chenzaomai.com/gtxiwhonxp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinqigfzy.top/gtruftyule.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinqigufen.top/gtevbnmswg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xylfe.cn/gtnvpdjyxw.html

[Q57] 行号
来源：http://hz.chenjidiqi.icu/gtcvkwgjgx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xuetiantiany.cn/gtsyrxquqv.html

[Q58] 累计求和
来源：http://hz.cqqwz.cn/gtbglmdymp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.haohaochexian.top/gtstkzwmbu.html

[Q59] 分组内累计
来源：http://hz.jinqigufen.top/gtmsvfnuug.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.316326.xyz/gtzptsldxr.html

[Q60] 取上一行 / 下一行
来源：http://hz.hywenlv.cn/gtkonjvwwk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.9152youxi.cn/gtvugyhjqd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.quarkkingdee.top/gtzggbfzxo.html

[Q61] 移动平均
来源：http://hz.meibo888.top/gtwwobkoiq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtxzdzkcnl.html

[Q62] 分组占比
来源：http://hz.mhx1999.top/gtqwfnymhi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sweek.top/gtqbunmtyj.html

[Q63] 开启事务
来源：http://hz.yongpay.top/gtwgkwedjx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jqgufenzy.top/gtkqpgdiqk.html

[Q64] 提交事务
来源：http://hz.snrcjt.cn/gtumysbtft.html

COMMIT;
来源：http://hz.guannengcc.top/gtiypclvqd.html

[Q65] 回滚事务
来源：http://hz.gotoacloud.top/gtnpcwmcnw.html

ROLLBACK;
来源：http://hz.sweek.top/gthvwtawbp.html

[Q66] 行锁查询
来源：http://hz.chenlongwang.top/gtjqquezio.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenjidiqi.icu/gtpgwpdsqj.html

[Q67] 设置隔离级别
来源：http://hz.xziqi.cn/gtvdwxpsin.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.andypj.xyz/gtfowozwvm.html

[Q68] 保存点
来源：http://hz.0kj1m.cn/gtmbeojvui.html

SAVEPOINT sp1;
来源：http://hz.xinyue.icu/gtoqywrquj.html

ROLLBACK TO sp1;
来源：http://hz.yonumen.top/gtkojemsih.html

[Q69] 查看执行计划
来源：http://hz.yanxiufei.cn/gtbepkzjyi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.redwolf501.top/gtyasifajd.html

[Q70] 更新统计信息
来源：http://hz.shzxlz.cn/gtpqerrytp.html

ANALYZE TABLE users;
来源：http://hz.shangyingyoupin.top/gtuodogoof.html

[Q71] 查看建表语句
来源：http://hz.svipenyu.cn/gtislwyued.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.redwolf501.top/gtfprcfcwo.html

[Q72] 查看索引
来源：http://hz.zhijiandao.cn/gtnenokpsh.html

SHOW INDEX FROM users;
来源：http://hz.zdqjudy.top/gtnapyervc.html

[Q73] 查看表状态
来源：http://hz.shangyingyoupin.top/gtkidmxiyy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yangfankeji.com/gttrupxirv.html

[Q74] 强制使用索引
来源：http://hz.yueranfly.top/gtgtoyxrrl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.gaohongyu789.top/gtcyynhjds.html

[Q75] 日期格式化
来源：http://hz.ydzc1.top/gtsykuwtvh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shanyushiyangtech.top/gtuctahial.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ppjwa.cn/gtzajwctjc.html

[Q76] 按天统计
来源：http://hz.yonumen.top/gtutyovjiw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.pycfn.com/gtljaszlbf.html

[Q77] 时间加减
来源：http://hz.zhaomingkeji.xyz/gtyaosimcq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.meibo888.top/gtqnrlngsb.html

[Q78] 当前时间
来源：http://hz.zhengqikj.top/gtvvefiwtn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ehwqpu.com/gtysfcvexn.html

[Q79] 字符串拼接
来源：http://hz.ppjwa.cn/gtkeqnmhtj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hammf.cn/gtbrheqviw.html

[Q80] 字符串截取
来源：http://hz.c1oappe.top/gtxncbncfv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ivvv.top/gtrlqrexrz.html

[Q81] 字符串替换
来源：http://hz.yj202588.top/gtlncqvauy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yj20258888.top/gtvaichlrb.html

[Q82] 字符长度与字节长度
来源：http://hz.jyoumei.cn/gtrjrjazxu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhijiandao.cn/gtqdtuvzli.html

[Q83] 大小写转换
来源：http://hz.cheryme.top/gtldxjvojx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhoulong.xyz/gtlokkafyv.html

[Q84] 去除首尾空格
来源：http://hz.yangfankeji.com/gtqgfnexki.html

SELECT TRIM(name) FROM users;
来源：http://hz.ydjk.org.cn/gtbrpyxwyc.html

[Q85] 数值取整
来源：http://hz.ydjk.org.cn/gtrecepqvq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xylfe.cn/gtjolhbcwl.html

[Q86] 读取 JSON 字段
来源：http://hz.zhengqikj.top/gtmcjjrvlo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.redwolf501.top/gtybxpwola.html

[Q87] JSON 字段做条件
来源：http://hz.cqqwz.cn/gtqujrdvts.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nanxinkj.top/gtljoyugqt.html

[Q88] 行转列（条件聚合）
来源：http://hz.havefunace.top/gtteppavup.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xingfuxueyuan.xyz/gttlbonydz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shzxlz.cn/gtkhnrlpwo.html

[Q89] 判断表是否存在
来源：http://hz.snrcjt.cn/gteuilndpc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cheryme.top/gtxbpelddw.html

[Q90] 生成序号列
来源：http://hz.snrcjt.cn/gtbckoffio.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cqqwz.cn/gtmolgdsae.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtgzsqqpel.html

R. Bash 专题
来源：http://hz.cdnleiting.top/gtzlufldgp.html

================================================================================
来源：http://hz.yuanzhike.top/gticruvrwi.html

[R01] shebang 与严格模式
来源：http://hz.sysykeji.top/gtqpmyvhrq.html

#!/usr/bin/env bash
来源：http://hz.pengpengdd.cyou/gtxrzquxvp.html

set -euo pipefail
来源：http://hz.jinyuanbaomall.cn/gtdlsvqtwt.html

[R02] 变量赋值与使用
来源：http://hz.aizwys.cn/gtsommthzm.html

name="Tom"; echo "$name"
来源：http://hz.sxryk.cn/gtbommzfbq.html

[R03] 只读变量
来源：http://hz.sxryk.cn/gtzlgtnhfj.html

readonly PI=3.14
来源：http://hz.hongshengwenyu.top/gthafbdbmp.html

[R04] 位置参数
来源：http://hz.zhaomingkeji.xyz/gtrhxpamnq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yongpay.top/gtvlgpsnay.html

[R05] 参数默认值
来源：http://hz.jinghuilouyu.cn/gtyndavxdn.html

name="${1:-default}"
来源：http://hz.zhoulong.xyz/gtdlvrhttt.html

[R06] 判断命令是否存在
来源：http://hz.zdqjudy.top/gtgnsenoct.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.316326.xyz/gtvnkejfbb.html

[R07] if 判断文件
来源：http://hz.tianlin.xyz/gtzwvscpfv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hnxiangtu.top/gtawjsdnaw.html

[R08] 数值比较
来源：http://hz.yanxiufei.cn/gtpwqobfnx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinyuanbaomall.cn/gtnapbbkmr.html

[R09] 字符串比较
来源：http://hz.fengsongda.top/gtxathmads.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhiwuduotai.top/gtnqcwibfj.html

[R10] 正则匹配
来源：http://hz.gogol.net.cn/gtxybiabus.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nanxuanxn.top/gtecgdcyur.html

[R11] case 多分支
来源：http://hz.ydjk.org.cn/gtyxwcsmpq.html

case "$1" in
来源：http://hz.pycfn.com/gtfmigpwiq.html

start) echo "启动" ;;
来源：http://hz.guowangkeji.top/gtzqlympjo.html

stop)  echo "停止" ;;
来源：http://hz.yuanzhike.top/gtdwmtbmov.html

*)     echo "未知命令" ;;
来源：http://hz.zhijiandao.cn/gticblslfe.html

esac
来源：http://hz.cheryme.top/gtzcypboui.html

[R12] for 遍历文件
来源：http://hz.kuanghao11.cn/gtzpyhxtyc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenzaomai.com/gtyrynvjgr.html

[R13] for 计数循环
来源：http://hz.ppjwa.cn/gtmxzteamg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ivvv.top/gtcweznyoe.html

[R14] C 风格 for
来源：http://hz.yj202588.top/gtqkzeczlv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.kuanghao11.cn/gtgbbhganp.html

[R15] while 逐行读文件
来源：http://hz.guannengcc.top/gtqbqwphzy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinghuilouyu.cn/gtzuaksraj.html

[R16] until 等待条件
来源：http://hz.wangdashe.top/gtzumajwuj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yvedp.cn/gtdajgzlxu.html

[R17] 数组定义与取值
来源：http://hz.tanke756.top/gtgzdhlbfo.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aibaodan.cn/gtogjaoouf.html

[R18] 遍历数组
来源：http://hz.nwbrower.top/gtytgiqdqm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhiwuduotai.top/gtupvayuni.html

[R19] 数组长度
来源：http://hz.gzhubu.top/gtubwqbgpk.html

echo "${#arr[@]}"
来源：http://hz.andypj.xyz/gtmzuxymmx.html

[R20] 关联数组（字典）
来源：http://hz.jqgufenzy.top/gtynlpuila.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.fengsongda.top/gtrnwgmcrs.html

[R21] 字符串长度
来源：http://hz.wangdashe.top/gtskcbgnin.html

echo "${#s}"
来源：http://hz.daria6918.cn/gtgpylmpkm.html

[R22] 截取子串
来源：http://hz.xuanzx.com/gtbwovbosn.html

echo "${s:0:5}"
来源：http://hz.cashguo.top/gtopfooszm.html

[R23] 字符串替换
来源：http://hz.aizwys.cn/gtfwdpnymp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hongshengwenyu.top/gtxozedote.html

[R24] 大小写转换
来源：http://hz.cashguo.top/gtdnffbtxe.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cheryme.top/gtigkktfpf.html

[R25] 去后缀 / 去前缀
来源：http://hz.nanxinkj.top/gtuzspooxs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yj20258.top/gtxlzcheuw.html

[R26] 命令替换
来源：http://hz.wangshuangyany.cn/gtmwjqspvb.html

now=$(date +%F); echo "$now"
来源：http://hz.yueranfly.top/gtthslvfgr.html

[R27] 算术展开
来源：http://hz.xinyue.icu/gtmqgajoib.html

echo $((1 + 2 * 3))
来源：http://hz.zhoulong.xyz/gtqanpbwzj.html

[R28] 浮点运算
来源：http://hz.sufxvd.cn/gtdztjudqi.html

echo "scale=2; 10/3" | bc
来源：http://hz.daria6918.cn/gtrmjhybfv.html

[R29] 定义函数
来源：http://hz.c1oappe.top/gtiwjijepk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.wangshuangyany.cn/gtbbjvqyrk.html

[R30] 函数返回状态码
来源：http://hz.bjfxy.top/gtcpuavbir.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nanxinkj.top/gtitjrtmil.html

[R31] 局部变量
来源：http://hz.shuidangran.top/gtxvpnpbqy.html

f() { local x=1; echo "$x"; }
来源：http://hz.sxryk.cn/gtuhkbmoxy.html

[R32] 参数个数校验
来源：http://hz.hammf.cn/gthxuityij.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hfpthk.cn/gtbbcexbgk.html

[R33] 捕获错误并提示行号
来源：http://hz.daria6918.cn/gtfvlwfunr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ppjwa.cn/gtzotcdbsk.html

[R34] 退出时清理
来源：http://hz.sxryk.cn/gtfjtzjagd.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shangyingyoupin.top/gtuwkcctbo.html

[R35] 后台执行并等待
来源：http://hz.jqgfzy.top/gteeiqcekk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinqigfzy.top/gtmzbeqxrn.html

[R36] 并发执行多个任务
来源：http://hz.wangdashe.top/gtkbayxiov.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.snrcjt.cn/gtxexrhqrm.html

[R37] 把输出赋给变量
来源：http://hz.yonumen.top/gtfbkepzlq.html

files=$(ls -1)
来源：http://hz.haohaochexian.top/gtfamecfma.html

[R38] 管道串联
来源：http://hz.0kj1m.cn/gtwobfancq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gzhubu.top/gtgbgxrbcq.html

[R39] 重定向标准输出与错误
来源：http://hz.xziqi.cn/gthdkrxqln.html

cmd > out.log 2>&1
来源：http://hz.c1oappe.top/gtgglnuwzm.html

[R40] 追加写日志
来源：http://hz.yanxiufei.cn/gtbodttvtl.html

echo "log" >> out.log
来源：http://hz.chenjidiqi.icu/gtqkzkkwbd.html

[R41] 丢弃输出
来源：http://hz.tianlin.xyz/gtrufkpyfu.html

cmd >/dev/null 2>&1
来源：http://hz.sxryk.cn/gtauviffqh.html

[R42] 输入重定向
来源：http://hz.yj202588.top/gtqipmpmca.html

wc -l < a.txt
来源：http://hz.nanxuanxn.top/gtyhnlooso.html

[R43] 按名字查找文件
来源：http://hz.tianlin.xyz/gtpojqinib.html

find . -name "*.log" -type f
来源：http://hz.cdnleiting.top/gtvqeikalu.html

[R44] 按修改时间查找
来源：http://hz.nwbrower.top/gtypjuvkbr.html

find . -mtime -7 -type f
来源：http://hz.c1oappe.top/gtyhbkgmpy.html

[R45] 批量删除
来源：http://hz.jianghu66.top/gtooampkib.html

find . -name "*.tmp" -delete
来源：http://hz.zhiwuduotai.top/gthanvbphk.html

[R46] 递归替换文件内容
来源：http://hz.feifeiyinyue.top/gtmyqmthmr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xuanzx.com/gtghotphal.html

[R47] sed 单行替换
来源：http://hz.daxiang520.top/gtwwhluzjc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.svipenyu.cn/gthcmwkxaw.html

[R48] awk 取指定列
来源：http://hz.xuetiantiany.cn/gtpkjtfiua.html

awk '{print $1, $3}' a.txt
来源：http://hz.dianchejie.cn/gtpovdzvnr.html

[R49] awk 带条件
来源：http://hz.sweek.top/gtwexfldyn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.daria6918.cn/gtoiylltqt.html

[R50] awk 求和
来源：http://hz.ehwqpu.com/gtjxjrpvod.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.snrcjt.cn/gtbvfmnraw.html

[R51] 排序去重取前几
来源：http://hz.hywenlv.cn/gtxkylxiil.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.mhx1999.top/gteipuhtwd.html

[R52] 统计行数
来源：http://hz.pengpengdd.cyou/gtylxbvrkh.html

wc -l a.txt
来源：http://hz.zhijiandao.cn/gtybgxjtwt.html

[R53] 查看文件头与实时尾
来源：http://hz.yanxiufei.cn/gtdairosva.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.havefunace.top/gtfsulpkbl.html

[R54] 比较两个文件
来源：http://hz.zdqjudy.top/gtersdsfku.html

diff a.txt b.txt
来源：http://hz.snrcjt.cn/gtfkwhzsvr.html

[R55] 压缩与解压
来源：http://hz.hammf.cn/gtslpblotx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tian-w.cn/gtoxkshvfp.html

[R56] 远程拷贝
来源：http://hz.guowangkeji.top/gtejostnmc.html

scp file user@host:/path/
来源：http://hz.yuxming.cn/gtyvuezgdi.html

[R57] 远程执行命令
来源：http://hz.zhijiandao.cn/gtvhkszwjz.html

ssh user@host 'uptime'
来源：http://hz.sufxvd.cn/gthcsmosyq.html

[R58] 下载文件
来源：http://hz.zhoulong.xyz/gtsctpeecn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.52xcode.cn/gtpnrqsfaj.html

[R59] 发 POST JSON
来源：http://hz.yvedp.cn/gtayzwaksx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shuidangran.top/gtulllczjj.html

[R60] 只看 HTTP 状态码
来源：http://hz.zycfv.cn/gtwnvsxrfv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ehwqpu.com/gtwhfyngbl.html

[R61] 磁盘占用
来源：http://hz.sufxvd.cn/gtzbvcutte.html

df -h;  du -sh *
来源：http://hz.smart0.xyz/gthdbzyqru.html

[R62] 找最占空间的文件
来源：http://hz.yongpay.top/gttpcrayrx.html

du -ah . | sort -rh | head -10
来源：http://hz.zhixingplan.top/gtdhmkqsyx.html

[R63] 内存与进程
来源：http://hz.jianghu66.top/gtjrvorkgw.html

free -h;  ps aux | grep nginx
来源：http://hz.zhaomingkeji.xyz/gtgvtndkzq.html

[R64] 结束进程
来源：http://hz.c1oappe.top/gtlmkruuwr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.pycfn.com/gtotoeauus.html

[R65] 查看端口占用
来源：http://hz.dianchejie.cn/gtfbqeemvj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hysaishi.cn/gtekhjutgw.html

[R66] 定时任务
来源：http://hz.chenlongwang.top/gtopbcxyaa.html

crontab -e;  crontab -l
来源：http://hz.jinyuanbaomall.cn/gtdkbejttb.html

[R67] 生成随机十六进制串
来源：http://hz.jinghuilouyu.cn/gtirrwxxpu.html

openssl rand -hex 16
来源：http://hz.pengpengdd.cyou/gtpnoomwrj.html

[R68] 计算文件校验值
来源：http://hz.shanyushiyangtech.top/gtkkyscffu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ydjk.org.cn/gtisieaptk.html

[R69] 生成随机密码
来源：http://hz.xingfuxueyuan.xyz/gtwxhincsc.html


<!-- 参考信息 -->