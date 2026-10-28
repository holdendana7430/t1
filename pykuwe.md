代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.haohaochexian.top/gtwwaalbxw.html

[Q18] 模糊匹配
来源：http://hz.haohaochexian.top/gtabxxzczj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhongyouzk.top/gtiruvrteq.html

[Q19] 范围查询
来源：http://hz.guannengcc.top/gtzateeytt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nanxuanxn.top/gtzqtmsilx.html

[Q20] IN 列表
来源：http://hz.xziqi.cn/gtczapwgzb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cdnleiting.top/gtmnapgpdx.html

[Q21] 空值判断
来源：http://hz.hnxiangtu.top/gtebippkue.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhongyouzk.top/gtjmpqodnk.html

[Q22] 排序
来源：http://hz.svipenyu.cn/gtmdchowtm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.meibo888.top/gtyjnjfsml.html

[Q23] 分页
来源：http://hz.yueranfly.top/gtndqrhmcs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.mhx1999.top/gtdtjrpbgj.html

[Q24] 去重
来源：http://hz.dashuyun.cn/gtdypdyvnp.html

SELECT DISTINCT city FROM users;
来源：http://hz.pengpengdd.cyou/gtmpznopvp.html

[Q25] 只取前 N 条
来源：http://hz.ydjk.org.cn/gtedjwsjeq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.birdmap.top/gthqvshmem.html

[Q26] 计数
来源：http://hz.pycfn.com/gtvtpumaks.html

SELECT COUNT(*) FROM users;
来源：http://hz.yangfankeji.com/gtgmfosfbf.html

[Q27] 条件计数
来源：http://hz.nanxinkj.top/gtpqfjngzg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ydjk.org.cn/gtlbdlasgm.html

[Q28] 求和与平均
来源：http://hz.yangfankeji.com/gtfcoyclbp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ivvv.top/gtxapelosf.html

[Q29] 最大最小值
来源：http://hz.birdmap.top/gtxdnmldyg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.wangshuangyany.cn/gttymtjiiq.html

[Q30] 分组统计
来源：http://hz.c1oappe.top/gtifrzntgi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.havefunace.top/gttxvefwqv.html

[Q31] 分组后过滤
来源：http://hz.yj20258.top/gtgmhyduzr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jyoumei.cn/gtdevkonqf.html

[Q32] 分组拼接字符串
来源：http://hz.wangdashe.top/gtskiavxnj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtfwtinobf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nanxinkj.top/gtsxcyerbm.html

[Q33] 多列分组
来源：http://hz.shuidangran.top/gtpiusdqwi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ywan-chungtsiang.top/gtcuzkubsn.html

[Q34] 每组取第一条
来源：http://hz.yueranfly.top/gtxorxauwz.html

SELECT * FROM (
来源：http://hz.gogol.net.cn/gtczsyrkjq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.9152youxi.cn/gtwmclhjke.html

) t WHERE rn = 1;
来源：http://hz.yueranfly.top/gtrekyitez.html

[Q35] 内连接
来源：http://hz.bjfxy.top/gtybvifemc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.aizwys.cn/gtiucoxiso.html

[Q36] 左连接
来源：http://hz.gotoacloud.top/gtetowkwcz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sxryk.cn/gtpyrsmcum.html

[Q37] 右连接
来源：http://hz.aizwys.cn/gthxhjqdlk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinqigufen.top/gtambhecdz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ydjk.org.cn/gttnswbihr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gzhubu.top/gttqbsyouy.html

[Q39] 自连接（查上下级）
来源：http://hz.yvedp.cn/gttiouzdiy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jyoumei.cn/gtahzjaupx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sufxvd.cn/gtbelefrqa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xylfe.cn/gtcdkamzin.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gzhubu.top/gtrvhlokyg.html

[Q41] 多表连接
来源：http://hz.cucudq.cn/gttigpibzy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.kuanghao11.cn/gtsqlqdvix.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhixingplan.top/gtniufdofm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yongpay.top/gtjwvejeyn.html

[Q42] 连接条件附加过滤
来源：http://hz.aibaodan.cn/gtucvhgark.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhengqikj.top/gtakcaeqjf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.smart0.xyz/gtycxmmxcg.html

[Q43] 标量子查询
来源：http://hz.yangfankeji.com/gtguldvmlh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.quarkkingdee.top/gtnamysdyj.html

[Q44] IN 子查询
来源：http://hz.xinyue.icu/gtgyndsooh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shzxlz.cn/gttvmryuth.html

[Q45] EXISTS 判断存在
来源：http://hz.yj202588.top/gtrguuawkk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cqqwz.cn/gtyhpcwwjj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jqgfzy.top/gtqtvkxwlt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258888.top/gtyrsqehlh.html

[Q47] 与平均值比较
来源：http://hz.cheryme.top/gtsmygjgpo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.kuanghao11.cn/gtijhoqqhb.html

[Q48] CTE 公用表表达式
来源：http://hz.hammf.cn/gtpfsjxvfs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zdqjudy.top/gtlztockcr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yongpay.top/gtbtyxppoa.html

[Q49] 更新单行
来源：http://hz.jlsjyb.cn/gthhmiwdqj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.bjfxy.top/gtarkmbtom.html

[Q50] 批量更新
来源：http://hz.aizwys.cn/gtsbafmaze.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.wangdashe.top/gtaheudtnz.html

[Q51] 用子查询更新
来源：http://hz.cucudq.cn/gtxznxkkmz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinqigufen.top/gtyiarsoxv.html

[Q52] 删除指定行
来源：http://hz.jinyuanbaomall.cn/gtojleuisz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.tianlin.xyz/gtxqrkavyy.html

[Q53] 按条件删除
来源：http://hz.sysykeji.top/gtcyfaghco.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ywan-chungtsiang.top/gthsohkbqo.html

[Q54] 清空表
来源：http://hz.wangshuangyany.cn/gtuowvuhdp.html

TRUNCATE TABLE logs;
来源：http://hz.tianlin.xyz/gtcefdotes.html

[Q55] 排名（并列占位）
来源：http://hz.gaohongyu789.top/gtladfhoyi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.wangshuangyany.cn/gtzzszkjde.html

[Q56] 密集排名（并列不占位）
来源：http://hz.birdmap.top/gtooaonqft.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.guannengcc.top/gtogzeikxw.html

[Q57] 行号
来源：http://hz.mhx1999.top/gtxtffoioc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhiwuduotai.top/gtfqmwxqmv.html

[Q58] 累计求和
来源：http://hz.tian-w.cn/gtjcajwkot.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yonumen.top/gtttueudiu.html

[Q59] 分组内累计
来源：http://hz.sufxvd.cn/gtgkcvpikf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.dashuyun.cn/gthtycrmej.html

[Q60] 取上一行 / 下一行
来源：http://hz.yj202588.top/gtcfbvdmvt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.guowangkeji.top/gtwizivvvo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yanxiufei.cn/gtlgfmtdxk.html

[Q61] 移动平均
来源：http://hz.guannengcc.top/gtjyewcwgr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gogol.net.cn/gtjjfpaizm.html

[Q62] 分组占比
来源：http://hz.aizwys.cn/gtztkutgfl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ehwqpu.com/gtcztgqmux.html

[Q63] 开启事务
来源：http://hz.hnxiangtu.top/gtnoyinbgx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.0kj1m.cn/gtyzfwrspo.html

[Q64] 提交事务
来源：http://hz.shanyushiyangtech.top/gtbajxowzm.html

COMMIT;
来源：http://hz.316326.xyz/gtxczoxxbu.html

[Q65] 回滚事务
来源：http://hz.aibaodan.cn/gtjetevhzp.html

ROLLBACK;
来源：http://hz.yanxiufei.cn/gtjedevfzj.html

[Q66] 行锁查询
来源：http://hz.zycfv.cn/gtfnaxbdzx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.birdmap.top/gtrzrtywsm.html

[Q67] 设置隔离级别
来源：http://hz.xuetiantiany.cn/gtyoimqeca.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.snrcjt.cn/gtbgntopgy.html

[Q68] 保存点
来源：http://hz.fengsongda.top/gtuuomlqvk.html

SAVEPOINT sp1;
来源：http://hz.jinqigufen.top/gtpxhboeki.html

ROLLBACK TO sp1;
来源：http://hz.hysaishi.cn/gtxqdpjozr.html

[Q69] 查看执行计划
来源：http://hz.fengsongda.top/gtivabpgto.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yanxiufei.cn/gtfmqycmjt.html

[Q70] 更新统计信息
来源：http://hz.xuetiantiany.cn/gtryxejmfe.html

ANALYZE TABLE users;
来源：http://hz.yangfankeji.com/gtotlaghtr.html

[Q71] 查看建表语句
来源：http://hz.sxryk.cn/gtctindepj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hysaishi.cn/gtwjshyont.html

[Q72] 查看索引
来源：http://hz.yj20258888.top/gtdcvjemnd.html

SHOW INDEX FROM users;
来源：http://hz.fengsongda.top/gtqtdyctms.html

[Q73] 查看表状态
来源：http://hz.nanxinkj.top/gttjcfyuot.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj202588.top/gtiajvutyo.html

[Q74] 强制使用索引
来源：http://hz.xuetiantiany.cn/gtrdwyiqxj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xylfe.cn/gtyrcckcns.html

[Q75] 日期格式化
来源：http://hz.gaohongyu789.top/gtxaqhuyut.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.dashuyun.cn/gtahkntdnw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhixingplan.top/gtmbduryiq.html

[Q76] 按天统计
来源：http://hz.dashuyun.cn/gtesibaphw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.wangdashe.top/gtyaqudmdg.html

[Q77] 时间加减
来源：http://hz.fengsongda.top/gtaxnkgdsw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinqigfzy.top/gtlfeauaxt.html

[Q78] 当前时间
来源：http://hz.feifeiyinyue.top/gtyjcvybtv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.chenjidiqi.icu/gtpcfxmpqq.html

[Q79] 字符串拼接
来源：http://hz.nanxuanxn.top/gtbkmccwmf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shuidangran.top/gtlykosnae.html

[Q80] 字符串截取
来源：http://hz.andypj.xyz/gtuxcfbqhb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtudnrorsg.html

[Q81] 字符串替换
来源：http://hz.yj202588.top/gtfzomdoxq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xuanzx.com/gtylnhsjwj.html

[Q82] 字符长度与字节长度
来源：http://hz.xinyue.icu/gtweovptjl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xziqi.cn/gtaaibovbg.html

[Q83] 大小写转换
来源：http://hz.jinqigufen.top/gtqbqkrtqk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yonumen.top/gtgeyrvlmb.html

[Q84] 去除首尾空格
来源：http://hz.smart0.xyz/gttswtcjbd.html

SELECT TRIM(name) FROM users;
来源：http://hz.hywenlv.cn/gtlfyzytoy.html

[Q85] 数值取整
来源：http://hz.zycfv.cn/gtmklbceox.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tanke756.top/gtaiznjegu.html

[Q86] 读取 JSON 字段
来源：http://hz.wangshuangyany.cn/gtdppbqmhs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenzaomai.com/gtubzxeqcq.html

[Q87] JSON 字段做条件
来源：http://hz.shzxlz.cn/gtxqdwzktf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nwbrower.top/gtavysfcoz.html

[Q88] 行转列（条件聚合）
来源：http://hz.tianlin.xyz/gtlikeuwji.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ydjk.org.cn/gtcqhkeuho.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yvedp.cn/gtjhqwfrkn.html

[Q89] 判断表是否存在
来源：http://hz.yj202588.top/gtejvyyjby.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yvedp.cn/gtetlshpbj.html

[Q90] 生成序号列
来源：http://hz.xuanzx.com/gtmivphhab.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zycfv.cn/gtezkzuxae.html

================================================================================
来源：http://hz.gaohongyu789.top/gtksbxgbfk.html

R. Bash 专题
来源：http://hz.gzhubu.top/gttjdgzjko.html

================================================================================
来源：http://hz.52xcode.cn/gtmnqhrkoy.html

[R01] shebang 与严格模式
来源：http://hz.bjfxy.top/gtexdsdxjg.html

#!/usr/bin/env bash
来源：http://hz.yangfankeji.com/gtvcrdfdzu.html

set -euo pipefail
来源：http://hz.cashguo.top/gtrrvgwjte.html

[R02] 变量赋值与使用
来源：http://hz.yj202588.top/gtwgheqpsz.html

name="Tom"; echo "$name"
来源：http://hz.zhoulong.xyz/gtoqnzwrcs.html

[R03] 只读变量
来源：http://hz.bjfxy.top/gtzdfanjwd.html

readonly PI=3.14
来源：http://hz.yvedp.cn/gtmnxlpiis.html

[R04] 位置参数
来源：http://hz.hnxiangtu.top/gtyqbyfccl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ybcxt.top/gtxcupvmkq.html

[R05] 参数默认值
来源：http://hz.chenzaomai.com/gtckwdlaof.html

name="${1:-default}"
来源：http://hz.guannengcc.top/gtydcumvie.html

[R06] 判断命令是否存在
来源：http://hz.yj202588.top/gtxzduvfnj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shanyushiyangtech.top/gtqltlvpuo.html

[R07] if 判断文件
来源：http://hz.aizwys.cn/gtgavpjzml.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jqgufenzy.top/gtmbzbivib.html

[R08] 数值比较
来源：http://hz.aibaodan.cn/gtmioqmxfl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sweek.top/gtxiqdgwvl.html

[R09] 字符串比较
来源：http://hz.xuanzx.com/gtzuojcwfk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhengqikj.top/gtontbxbob.html

[R10] 正则匹配
来源：http://hz.yonumen.top/gtkktxyqnn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nwbrower.top/gtmzfzawbg.html

[R11] case 多分支
来源：http://hz.jiagoushi.top/gtbkyswsaa.html

case "$1" in
来源：http://hz.chenzaomai.com/gtwjnzzfnx.html

start) echo "启动" ;;
来源：http://hz.shuidangran.top/gtvrvihdjx.html

stop)  echo "停止" ;;
来源：http://hz.zycfv.cn/gtdfthmyup.html

*)     echo "未知命令" ;;
来源：http://hz.pengpengdd.cyou/gtzmswfijr.html

esac
来源：http://hz.aibaodan.cn/gtbnduszav.html

[R12] for 遍历文件
来源：http://hz.kuanghao11.cn/gtgyehbscp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.nwbrower.top/gtmqggqjhh.html

[R13] for 计数循环
来源：http://hz.bjfxy.top/gtaxuwgkvh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhoulong.xyz/gtderkfmpi.html

[R14] C 风格 for
来源：http://hz.zhengqikj.top/gteqhdoyhl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj20258888.top/gtaaqwfdot.html

[R15] while 逐行读文件
来源：http://hz.jqgufenzy.top/gtfomeucfg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.pengpengdd.cyou/gtzswewfxu.html

[R16] until 等待条件
来源：http://hz.havefunace.top/gtjfthauhb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtwfqivefg.html

[R17] 数组定义与取值
来源：http://hz.yvedp.cn/gtbkdgqvfa.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.havefunace.top/gtuvywglcg.html

[R18] 遍历数组
来源：http://hz.hysaishi.cn/gtpnrnqmxi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhaomingkeji.xyz/gtvffvwscm.html

[R19] 数组长度
来源：http://hz.c1oappe.top/gtnkzyhkfq.html

echo "${#arr[@]}"
来源：http://hz.feifeiyinyue.top/gtrkbiizip.html

[R20] 关联数组（字典）
来源：http://hz.hfpthk.cn/gtvpaewesh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cheryme.top/gtvkqxtgwz.html

[R21] 字符串长度
来源：http://hz.cashguo.top/gtydazegai.html

echo "${#s}"
来源：http://hz.jinyuanbaomall.cn/gtlckwaene.html

[R22] 截取子串
来源：http://hz.zhengqikj.top/gtekitlzbg.html

echo "${s:0:5}"
来源：http://hz.quarkkingdee.top/gtdridcxdr.html

[R23] 字符串替换
来源：http://hz.cqqwz.cn/gtursfrkkl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xylfe.cn/gtkyfqwdpc.html

[R24] 大小写转换
来源：http://hz.xylfe.cn/gtmfxqngdk.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sufxvd.cn/gtqbnwsvaf.html

[R25] 去后缀 / 去前缀
来源：http://hz.hywenlv.cn/gtjyungvan.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sweek.top/gtouoffpch.html

[R26] 命令替换
来源：http://hz.shanyushiyangkeji.top/gttnifmazd.html

now=$(date +%F); echo "$now"
来源：http://hz.chenzaomai.com/gtefmmfkwl.html

[R27] 算术展开
来源：http://hz.redwolf501.top/gtdyqejmml.html

echo $((1 + 2 * 3))
来源：http://hz.jinghuilouyu.cn/gtovkaghrl.html

[R28] 浮点运算
来源：http://hz.chenlongwang.top/gtmwddqhth.html

echo "scale=2; 10/3" | bc
来源：http://hz.guowangkeji.top/gthnzelkze.html

[R29] 定义函数
来源：http://hz.pengpengdd.cyou/gtbfctfhiw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nwbrower.top/gtfzcxnmsm.html

[R30] 函数返回状态码
来源：http://hz.wangdashe.top/gtbvlteupl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.quarkkingdee.top/gtdfxutlrw.html

[R31] 局部变量
来源：http://hz.hongshengwenyu.top/gtazuvhggd.html

f() { local x=1; echo "$x"; }
来源：http://hz.316326.xyz/gthlmwsbpo.html

[R32] 参数个数校验
来源：http://hz.shanyushiyangtech.top/gtknvvwmdo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jlsjyb.cn/gtjucmpqmg.html

[R33] 捕获错误并提示行号
来源：http://hz.zhixingplan.top/gtcsmpuqat.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.wangshuangyany.cn/gtwaflgevw.html

[R34] 退出时清理
来源：http://hz.nwbrower.top/gtolqgbmsy.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtgykkgmow.html

[R35] 后台执行并等待
来源：http://hz.jinghuilouyu.cn/gtprkkxdwu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinqigfzy.top/gtvwwgwxvz.html

[R36] 并发执行多个任务
来源：http://hz.zycfv.cn/gtyiasepws.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tian-w.cn/gteftixcnc.html

[R37] 把输出赋给变量
来源：http://hz.fzhhl.top/gtzwmwxrly.html

files=$(ls -1)
来源：http://hz.svipenyu.cn/gttnhuvegr.html

[R38] 管道串联
来源：http://hz.meibo888.top/gtwwrbsykf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hammf.cn/gtxipildue.html

[R39] 重定向标准输出与错误
来源：http://hz.havefunace.top/gtxsdbeqnj.html

cmd > out.log 2>&1
来源：http://hz.xingfuxueyuan.xyz/gtlfmrevxc.html

[R40] 追加写日志
来源：http://hz.aizwys.cn/gtfqsdtrwh.html

echo "log" >> out.log
来源：http://hz.sufxvd.cn/gtahtqtqif.html

[R41] 丢弃输出
来源：http://hz.smart0.xyz/gtvotmnebq.html

cmd >/dev/null 2>&1
来源：http://hz.svipenyu.cn/gtixsagpva.html

[R42] 输入重定向
来源：http://hz.ybcxt.top/gtpfxueunc.html

wc -l < a.txt
来源：http://hz.wangdashe.top/gtgltkstue.html

[R43] 按名字查找文件
来源：http://hz.tian-w.cn/gtvigxhnoo.html

find . -name "*.log" -type f
来源：http://hz.sweek.top/gthcirngmr.html

[R44] 按修改时间查找
来源：http://hz.andypj.xyz/gthpunpyes.html

find . -mtime -7 -type f
来源：http://hz.ydzc1.top/gtnudbzrbr.html

[R45] 批量删除
来源：http://hz.9152youxi.cn/gtjvlomztf.html

find . -name "*.tmp" -delete
来源：http://hz.kuanghao11.cn/gtpovkvpto.html

[R46] 递归替换文件内容
来源：http://hz.yanxiufei.cn/gtgwkdefav.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.fengsongda.top/gtxtwlkqiw.html

[R47] sed 单行替换
来源：http://hz.ivvv.top/gtwmkvhykt.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.aibaodan.cn/gtfajigqnp.html

[R48] awk 取指定列
来源：http://hz.cucudq.cn/gtjwvirbwn.html

awk '{print $1, $3}' a.txt
来源：http://hz.jianghu66.top/gtqlrklnja.html

[R49] awk 带条件
来源：http://hz.xingfuxueyuan.xyz/gtjyhtapmb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.wangdashe.top/gtqospayun.html

[R50] awk 求和
来源：http://hz.cucudq.cn/gtjwngvwva.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.snrcjt.cn/gtwrtlufiz.html

[R51] 排序去重取前几
来源：http://hz.iojbl.cn/gtwexloxsv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gogol.net.cn/gthqlkmkyh.html

[R52] 统计行数
来源：http://hz.feifeiyinyue.top/gtvwanmyei.html

wc -l a.txt
来源：http://hz.yj20258.top/gtvvbbuavf.html

[R53] 查看文件头与实时尾
来源：http://hz.kuanghao11.cn/gteipmleam.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hysaishi.cn/gtatnbncls.html

[R54] 比较两个文件
来源：http://hz.gaohongyu789.top/gtdiwqxhtv.html

diff a.txt b.txt
来源：http://hz.xylfe.cn/gtonfcliyb.html

[R55] 压缩与解压
来源：http://hz.jinqigfzy.top/gtxsttfxhg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yonumen.top/gtdwvywfzo.html

[R56] 远程拷贝
来源：http://hz.hnqzz.top/gtyhdldxoj.html

scp file user@host:/path/
来源：http://hz.haohaochexian.top/gtrmoyivcq.html

[R57] 远程执行命令
来源：http://hz.zycfv.cn/gtypmaxhog.html

ssh user@host 'uptime'
来源：http://hz.xziqi.cn/gtgfnvymnq.html

[R58] 下载文件
来源：http://hz.chenjidiqi.icu/gttjcmkivt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ywan-chungtsiang.top/gtctsrnoop.html

[R59] 发 POST JSON
来源：http://hz.ydjk.org.cn/gtsuexoiev.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shuidangran.top/gtigtyrkpc.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj202588.top/gtlcwrqldu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ehwqpu.com/gtlvqpqsxt.html

[R61] 磁盘占用
来源：http://hz.cashguo.top/gtaojpkiac.html

df -h;  du -sh *
来源：http://hz.nwbrower.top/gthwmhxgqt.html

[R62] 找最占空间的文件
来源：http://hz.xziqi.cn/gtvxltrfhl.html

du -ah . | sort -rh | head -10
来源：http://hz.fengsongda.top/gthhbblpjh.html

[R63] 内存与进程
来源：http://hz.yongpay.top/gtdylxchci.html

free -h;  ps aux | grep nginx
来源：http://hz.ppjwa.cn/gtpbykuzqr.html

[R64] 结束进程
来源：http://hz.ivvv.top/gtawsnpjyd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.iojbl.cn/gtrjujjujv.html

[R65] 查看端口占用
来源：http://hz.zycfv.cn/gtwxafuurr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hammf.cn/gttnvbhysp.html

[R66] 定时任务
来源：http://hz.tanke756.top/gtaoqabvgp.html

crontab -e;  crontab -l
来源：http://hz.fzhhl.top/gthwfuxoay.html

[R67] 生成随机十六进制串
来源：http://hz.yj20258888.top/gtscbaiswd.html


<!-- 参考信息 -->