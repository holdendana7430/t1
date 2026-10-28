代发 wailian999

SELECT * FROM users;
来源：http://hz.yanxiufei.cn/gtwrnwdoko.html

[Q16] 查询指定列
来源：http://hz.vqdsnc.cn/gtoboxapky.html

SELECT id, name FROM users;
来源：http://hz.pycfn.com/gtfxiqzgjc.html

[Q17] 条件查询
来源：http://hz.yonumen.top/gtecwhduam.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ydjk.org.cn/gtqvylmwbk.html

[Q18] 模糊匹配
来源：http://hz.wangshuangyany.cn/gtdrxrrrul.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hongshengwenyu.top/gtziyozsyo.html

[Q19] 范围查询
来源：http://hz.xinyue.icu/gtehkqrlmh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yueranfly.top/gtygqxawmw.html

[Q20] IN 列表
来源：http://hz.zdqjudy.top/gtywubrfrs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ydzc1.top/gtayaprcfj.html

[Q21] 空值判断
来源：http://hz.vqdsnc.cn/gtzccdxrwp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yonumen.top/gtspuaxutn.html

[Q22] 排序
来源：http://hz.jqgfzy.top/gtjopwaexy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.meibo888.top/gthuznvstk.html

[Q23] 分页
来源：http://hz.sweek.top/gtoawqoory.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jiagoushi.top/gtxueeqhmo.html

[Q24] 去重
来源：http://hz.cdnleiting.top/gttbjeidda.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhengqikj.top/gtqyztlqzv.html

[Q25] 只取前 N 条
来源：http://hz.shangyingyoupin.top/gtoieecugw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.nanxuanxn.top/gteljmvvxk.html

[Q26] 计数
来源：http://hz.jinqigfzy.top/gtqgsxczbp.html

SELECT COUNT(*) FROM users;
来源：http://hz.shzxlz.cn/gtffaqkbbr.html

[Q27] 条件计数
来源：http://hz.feifeiyinyue.top/gtpxbddcqh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhengqikj.top/gtyefnrxyb.html

[Q28] 求和与平均
来源：http://hz.ydjk.org.cn/gtsdugrpmg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cheryme.top/gtqxrwasvg.html

[Q29] 最大最小值
来源：http://hz.cqqwz.cn/gtbkwbzscp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.snrcjt.cn/gtdifgmxar.html

[Q30] 分组统计
来源：http://hz.zhaomingkeji.xyz/gtpyflplcu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yuxming.cn/gtfhjtkxzu.html

[Q31] 分组后过滤
来源：http://hz.zhijiandao.cn/gtobrlgrza.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ydjk.org.cn/gtjmiaysrf.html

[Q32] 分组拼接字符串
来源：http://hz.xziqi.cn/gtcgikxbha.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtaavevqif.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yj202588.top/gtymokesgp.html

[Q33] 多列分组
来源：http://hz.shzxlz.cn/gtvijluwns.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yonumen.top/gtnfwkpuca.html

[Q34] 每组取第一条
来源：http://hz.xuetiantiany.cn/gtkxlyjoci.html

SELECT * FROM (
来源：http://hz.gogol.net.cn/gtfeulbmtg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.nanxuanxn.top/gtspejwqvv.html

) t WHERE rn = 1;
来源：http://hz.aizwys.cn/gtkchkkcir.html

[Q35] 内连接
来源：http://hz.quarkkingdee.top/gttldjhxmf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hfpthk.cn/gtydxpgzwm.html

[Q36] 左连接
来源：http://hz.bjfxy.top/gtrdutvpdb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jianghu66.top/gtddnvears.html

[Q37] 右连接
来源：http://hz.ydjk.org.cn/gtyawfqjrl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.iojbl.cn/gtkvahgygr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.quarkkingdee.top/gtutefqhgv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.dashuyun.cn/gtbldcjvxg.html

[Q39] 自连接（查上下级）
来源：http://hz.svipenyu.cn/gtovnasnka.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xylfe.cn/gtkkkxipcu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhoulong.xyz/gteoyqgnoz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jlsjyb.cn/gticoxnkla.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sysykeji.top/gtxaazrsht.html

[Q41] 多表连接
来源：http://hz.yj20258888.top/gtllnfutpe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tian-w.cn/gtlhobksxv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sysykeji.top/gtilewwxoq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.wangdashe.top/gtxrlhrkuh.html

[Q42] 连接条件附加过滤
来源：http://hz.cashguo.top/gtlrqcjxuh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cqqwz.cn/gtyhofkzbx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shangyingyoupin.top/gtwxkajiaw.html

[Q43] 标量子查询
来源：http://hz.xuetiantiany.cn/gtqjrbwiyf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.mhx1999.top/gtzxyzfjfh.html

[Q44] IN 子查询
来源：http://hz.feifeiyinyue.top/gtoyodjvdg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hammf.cn/gtcooxzags.html

[Q45] EXISTS 判断存在
来源：http://hz.jinqigufen.top/gtcrcyqavo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shzxlz.cn/gtrmjvbovj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xuetiantiany.cn/gtuevddcdu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guowangkeji.top/gtttvrefpg.html

[Q47] 与平均值比较
来源：http://hz.shanyushiyangkeji.top/gtzlpjhmvs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhiwuduotai.top/gtiogwdvkq.html

[Q48] CTE 公用表表达式
来源：http://hz.ydjk.org.cn/gtpgerupad.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yueranfly.top/gtjihyijbd.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.nanxuanxn.top/gttrporguf.html

[Q49] 更新单行
来源：http://hz.cucudq.cn/gtspimnsvg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.fzhhl.top/gtjtmjtaga.html

[Q50] 批量更新
来源：http://hz.birdmap.top/gtizvmhgvc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.0kj1m.cn/gttpezfpaf.html

[Q51] 用子查询更新
来源：http://hz.hammf.cn/gtmkewubyp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.fzhhl.top/gtumvnjzhf.html

[Q52] 删除指定行
来源：http://hz.jlsjyb.cn/gtmhgccgbp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ppjwa.cn/gtdvkolswi.html

[Q53] 按条件删除
来源：http://hz.fengsongda.top/gtokbjfcwk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cheryme.top/gtfcqohkyr.html

[Q54] 清空表
来源：http://hz.0kj1m.cn/gtqsserhns.html

TRUNCATE TABLE logs;
来源：http://hz.zhongyouzk.top/gtkcxdsjsl.html

[Q55] 排名（并列占位）
来源：http://hz.sysykeji.top/gtkpvdupdw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shanyushiyangkeji.top/gtteqgwcsi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zdqjudy.top/gtdkbdlipn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sysykeji.top/gtzpinrwdr.html

[Q57] 行号
来源：http://hz.hnxiangtu.top/gtxpbwklxz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.meibo888.top/gtjatrljaj.html

[Q58] 累计求和
来源：http://hz.yuanzhike.top/gtrucrqjgg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.quarkkingdee.top/gtlsqwhoqv.html

[Q59] 分组内累计
来源：http://hz.guowangkeji.top/gtgkgmeiga.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xylfe.cn/gtvhqhhegy.html

[Q60] 取上一行 / 下一行
来源：http://hz.jianghu66.top/gtxiksasge.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yongpay.top/gtjihmfjuw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenzaomai.com/gtwkuwgcvu.html

[Q61] 移动平均
来源：http://hz.hywenlv.cn/gtibwcblqx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.tianlin.xyz/gtkkgaiycf.html

[Q62] 分组占比
来源：http://hz.zhaomingkeji.xyz/gtojdoldxa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.316326.xyz/gtuihhevyr.html

[Q63] 开启事务
来源：http://hz.bjfxy.top/gtmwrzvfjs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxinkj.top/gtbnafyodw.html

[Q64] 提交事务
来源：http://hz.tianlin.xyz/gtsaswdhfi.html

COMMIT;
来源：http://hz.yj20258.top/gtkteclhre.html

[Q65] 回滚事务
来源：http://hz.chenlongwang.top/gtcssnavoq.html

ROLLBACK;
来源：http://hz.nanxuanxn.top/gttxjcmilp.html

[Q66] 行锁查询
来源：http://hz.aibaodan.cn/gtdgmbytfh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hfpthk.cn/gtdxtckwrt.html

[Q67] 设置隔离级别
来源：http://hz.zhoulong.xyz/gtekoycpau.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.daxiang520.top/gtqnagaohb.html

[Q68] 保存点
来源：http://hz.yj20258888.top/gtmpsuxftx.html

SAVEPOINT sp1;
来源：http://hz.wangshuangyany.cn/gtkxlpupoe.html

ROLLBACK TO sp1;
来源：http://hz.cashguo.top/gtvhmeafht.html

[Q69] 查看执行计划
来源：http://hz.zhoulong.xyz/gtozclebhn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jianghu66.top/gtmrqdalbu.html

[Q70] 更新统计信息
来源：http://hz.pengpengdd.cyou/gtywvhofkw.html

ANALYZE TABLE users;
来源：http://hz.xingfuxueyuan.xyz/gtfzdluwmp.html

[Q71] 查看建表语句
来源：http://hz.tanke756.top/gtsnpuoeas.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.redwolf501.top/gtajttpver.html

[Q72] 查看索引
来源：http://hz.gogol.net.cn/gtagmrbbdb.html

SHOW INDEX FROM users;
来源：http://hz.chenjidiqi.icu/gtkwdjhvzh.html

[Q73] 查看表状态
来源：http://hz.yueranfly.top/gttbjyhxxs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.aibaodan.cn/gtarcarvkx.html

[Q74] 强制使用索引
来源：http://hz.redwolf501.top/gtxhzsendn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.gotoacloud.top/gtdvpihtfq.html

[Q75] 日期格式化
来源：http://hz.bjfxy.top/gtbqzculdp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.pycfn.com/gtduofiqrr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.guowangkeji.top/gtimlunfpk.html

[Q76] 按天统计
来源：http://hz.redwolf501.top/gtrsfvqhvw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.0kj1m.cn/gtcyxzqvps.html

[Q77] 时间加减
来源：http://hz.meibo888.top/gtufamripk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenjidiqi.icu/gtbztrhswi.html

[Q78] 当前时间
来源：http://hz.yuanzhike.top/gtghduxvsi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yanxiufei.cn/gtygcmqcac.html

[Q79] 字符串拼接
来源：http://hz.cdnleiting.top/gtyleqlhga.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jqgfzy.top/gtbypcvqwy.html

[Q80] 字符串截取
来源：http://hz.cdnleiting.top/gtaunacioq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.fengsongda.top/gtxucmhcad.html

[Q81] 字符串替换
来源：http://hz.dianchejie.cn/gtmqdrgnal.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.guannengcc.top/gtyafzipft.html

[Q82] 字符长度与字节长度
来源：http://hz.sysykeji.top/gtwsdqipqw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yvedp.cn/gtccugncko.html

[Q83] 大小写转换
来源：http://hz.zhaomingkeji.xyz/gtypgkgzaz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zycfv.cn/gtbjglsvet.html

[Q84] 去除首尾空格
来源：http://hz.nwbrower.top/gtnviwqakh.html

SELECT TRIM(name) FROM users;
来源：http://hz.sysykeji.top/gtszwtzxuf.html

[Q85] 数值取整
来源：http://hz.shanyushiyangkeji.top/gtjxwhfsde.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.chenzaomai.com/gtvwlyelzj.html

[Q86] 读取 JSON 字段
来源：http://hz.yj20258.top/gtvhvionri.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.meibo888.top/gttksmmoai.html

[Q87] JSON 字段做条件
来源：http://hz.redwolf501.top/gtffzliais.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinqigufen.top/gtewyqadqw.html

[Q88] 行转列（条件聚合）
来源：http://hz.gaohongyu789.top/gtcmjdzrok.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ydjk.org.cn/gtohnodcfz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gaohongyu789.top/gtxhkomwdl.html

[Q89] 判断表是否存在
来源：http://hz.ehwqpu.com/gtbckfwvyq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhoulong.xyz/gtpimjbusw.html

[Q90] 生成序号列
来源：http://hz.316326.xyz/gtvkewlmcf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.pycfn.com/gtmrhlckbp.html

================================================================================
来源：http://hz.zycfv.cn/gtfhrjdvsp.html

R. Bash 专题
来源：http://hz.havefunace.top/gttzgvgiil.html

================================================================================
来源：http://hz.ydzc1.top/gtvgblrxqk.html

[R01] shebang 与严格模式
来源：http://hz.jinyuanbaomall.cn/gtzpxhgbga.html

#!/usr/bin/env bash
来源：http://hz.pengpengdd.cyou/gtcggicret.html

set -euo pipefail
来源：http://hz.fzhhl.top/gtqljgdcyn.html

[R02] 变量赋值与使用
来源：http://hz.fengsongda.top/gtcalcjtcy.html

name="Tom"; echo "$name"
来源：http://hz.havefunace.top/gtknqxvmur.html

[R03] 只读变量
来源：http://hz.haohaochexian.top/gtzzcjrvvc.html

readonly PI=3.14
来源：http://hz.ywan-chungtsiang.top/gtzlwtbfkr.html

[R04] 位置参数
来源：http://hz.hysaishi.cn/gtdjlhwcya.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhijiandao.cn/gtxghyowhc.html

[R05] 参数默认值
来源：http://hz.hywenlv.cn/gtegyutdxd.html

name="${1:-default}"
来源：http://hz.haohaochexian.top/gtqiopbijl.html

[R06] 判断命令是否存在
来源：http://hz.yonumen.top/gtkmmsczdz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jyoumei.cn/gtydyyrrln.html

[R07] if 判断文件
来源：http://hz.shangyingyoupin.top/gtrzvjsisy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.fzhhl.top/gttxdqwrcp.html

[R08] 数值比较
来源：http://hz.ydjk.org.cn/gtutnybrps.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.52xcode.cn/gtqanlhjlu.html

[R09] 字符串比较
来源：http://hz.jinyuanbaomall.cn/gteqdheswh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhijiandao.cn/gtritfjmqn.html

[R10] 正则匹配
来源：http://hz.daxiang520.top/gtzjddxdto.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sweek.top/gtoiruccrv.html

[R11] case 多分支
来源：http://hz.hnqzz.top/gtdygrbekx.html

case "$1" in
来源：http://hz.yvedp.cn/gtsyoncget.html

start) echo "启动" ;;
来源：http://hz.jqgfzy.top/gtzqerxwsl.html

stop)  echo "停止" ;;
来源：http://hz.ppjwa.cn/gtvcnqqldq.html

*)     echo "未知命令" ;;
来源：http://hz.xuanzx.com/gtmgfknvwx.html

esac
来源：http://hz.wangshuangyany.cn/gtbofgkhjr.html

[R12] for 遍历文件
来源：http://hz.cheryme.top/gtlqmvnqaw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gotoacloud.top/gtwmqrwwaq.html

[R13] for 计数循环
来源：http://hz.zycfv.cn/gtldyvnlzo.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.c1oappe.top/gtycpqhxef.html

[R14] C 风格 for
来源：http://hz.gogol.net.cn/gthedcpnhh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hfpthk.cn/gtdhugzjur.html

[R15] while 逐行读文件
来源：http://hz.zycfv.cn/gtwcorzanb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jiagoushi.top/gtkhgbvkpu.html

[R16] until 等待条件
来源：http://hz.xingfuxueyuan.xyz/gtlxuoajod.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinyuanbaomall.cn/gtjpyzamql.html

[R17] 数组定义与取值
来源：http://hz.jlsjyb.cn/gtmprbkupv.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenjidiqi.icu/gtdeiuwten.html

[R18] 遍历数组
来源：http://hz.ehwqpu.com/gtezeoactj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jqgufenzy.top/gtdueradal.html

[R19] 数组长度
来源：http://hz.tian-w.cn/gtxgejoesf.html

echo "${#arr[@]}"
来源：http://hz.mhx1999.top/gtonvodmnp.html

[R20] 关联数组（字典）
来源：http://hz.mhx1999.top/gtmlpshpna.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.andypj.xyz/gtqznbqjkv.html

[R21] 字符串长度
来源：http://hz.xziqi.cn/gtpnpnfezi.html

echo "${#s}"
来源：http://hz.gaohongyu789.top/gttzdmrcxo.html

[R22] 截取子串
来源：http://hz.xuanzx.com/gtxfxiyjkm.html

echo "${s:0:5}"
来源：http://hz.hammf.cn/gtxerittlh.html

[R23] 字符串替换
来源：http://hz.ybcxt.top/gtmhzktfgj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hysaishi.cn/gtkbistujs.html

[R24] 大小写转换
来源：http://hz.yonumen.top/gtwbbwxeqa.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.pycfn.com/gtshlhfsnd.html

[R25] 去后缀 / 去前缀
来源：http://hz.wangshuangyany.cn/gtunngpukd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.aibaodan.cn/gtlebvyjes.html

[R26] 命令替换
来源：http://hz.birdmap.top/gtfxtizmje.html

now=$(date +%F); echo "$now"
来源：http://hz.jqgufenzy.top/gtmgtlokrg.html

[R27] 算术展开
来源：http://hz.zhijiandao.cn/gtmxnajkye.html

echo $((1 + 2 * 3))
来源：http://hz.tianlin.xyz/gtszipxgko.html

[R28] 浮点运算
来源：http://hz.hammf.cn/gtvksirafi.html

echo "scale=2; 10/3" | bc
来源：http://hz.zycfv.cn/gtcouwzigc.html

[R29] 定义函数
来源：http://hz.yj202588.top/gthexkuhcp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jqgufenzy.top/gtfwfjjayp.html

[R30] 函数返回状态码
来源：http://hz.zhoulong.xyz/gtuhlvqclx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.vqdsnc.cn/gtnxpsndae.html

[R31] 局部变量
来源：http://hz.aizwys.cn/gtqkzlkurs.html

f() { local x=1; echo "$x"; }
来源：http://hz.tian-w.cn/gtswqjhtui.html

[R32] 参数个数校验
来源：http://hz.shuidangran.top/gtzcvdjhim.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hywenlv.cn/gtomicqbcj.html

[R33] 捕获错误并提示行号
来源：http://hz.jlsjyb.cn/gtmiogjgxc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jyoumei.cn/gtwfztvjyk.html

[R34] 退出时清理
来源：http://hz.xinyue.icu/gtamxycrkk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shuidangran.top/gtuwponykf.html

[R35] 后台执行并等待
来源：http://hz.xuetiantiany.cn/gtfiuyajfk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.vqdsnc.cn/gtsdhzifea.html

[R36] 并发执行多个任务
来源：http://hz.zycfv.cn/gtxcnndvfc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yongpay.top/gtdrrtojec.html

[R37] 把输出赋给变量
来源：http://hz.tian-w.cn/gtvgszlqpt.html

files=$(ls -1)
来源：http://hz.fzhhl.top/gtaxafkqfi.html

[R38] 管道串联
来源：http://hz.shangyingyoupin.top/gtmhsurnwk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhixingplan.top/gtreonfbuk.html

[R39] 重定向标准输出与错误
来源：http://hz.ydjk.org.cn/gtyzbwookj.html

cmd > out.log 2>&1
来源：http://hz.ybcxt.top/gtepgdiypx.html

[R40] 追加写日志
来源：http://hz.jlsjyb.cn/gtodcorkqq.html

echo "log" >> out.log
来源：http://hz.yanxiufei.cn/gtbdfgxjby.html

[R41] 丢弃输出
来源：http://hz.yj20258.top/gtesfmgdbl.html

cmd >/dev/null 2>&1
来源：http://hz.52xcode.cn/gtcpjggijk.html

[R42] 输入重定向
来源：http://hz.meibo888.top/gtyzeovtpb.html

wc -l < a.txt
来源：http://hz.shanyushiyangtech.top/gthfhonhda.html

[R43] 按名字查找文件
来源：http://hz.jianghu66.top/gtafeniutj.html

find . -name "*.log" -type f
来源：http://hz.tianlin.xyz/gtwnimcfgm.html

[R44] 按修改时间查找
来源：http://hz.zhaomingkeji.xyz/gtucefccpi.html

find . -mtime -7 -type f
来源：http://hz.ywan-chungtsiang.top/gtljguearz.html

[R45] 批量删除
来源：http://hz.guannengcc.top/gtazvvpiwd.html

find . -name "*.tmp" -delete
来源：http://hz.dashuyun.cn/gtkviqfswv.html

[R46] 递归替换文件内容
来源：http://hz.chenlongwang.top/gtuqxfrlvy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xziqi.cn/gtdjhxubix.html

[R47] sed 单行替换
来源：http://hz.hnqzz.top/gtzmuyohqz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shangyingyoupin.top/gtucjmofzi.html

[R48] awk 取指定列
来源：http://hz.yongpay.top/gtwofghyir.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhongyouzk.top/gtqfpresei.html

[R49] awk 带条件
来源：http://hz.zhiwuduotai.top/gtkuntgzgu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ydjk.org.cn/gtupkhfsvo.html

[R50] awk 求和
来源：http://hz.xuanzx.com/gtqqhxvgkl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ivvv.top/gtxnjppkak.html

[R51] 排序去重取前几
来源：http://hz.zycfv.cn/gtzyfmgkdb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.quarkkingdee.top/gtztyvyslq.html

[R52] 统计行数
来源：http://hz.0kj1m.cn/gtwwaomnxe.html

wc -l a.txt
来源：http://hz.cucudq.cn/gtvdgtmtaf.html

[R53] 查看文件头与实时尾
来源：http://hz.chenlongwang.top/gtlhcchhvd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xziqi.cn/gtorynfgol.html

[R54] 比较两个文件
来源：http://hz.yj20258888.top/gtuvmdpkqb.html

diff a.txt b.txt
来源：http://hz.nwbrower.top/gtnvqgesul.html

[R55] 压缩与解压
来源：http://hz.cheryme.top/gtmrpkvgdi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.wangdashe.top/gtsupnzfwj.html

[R56] 远程拷贝
来源：http://hz.zhiwuduotai.top/gtmlqrmgir.html

scp file user@host:/path/
来源：http://hz.shzxlz.cn/gteaximghb.html

[R57] 远程执行命令
来源：http://hz.svipenyu.cn/gtzphxmdre.html

ssh user@host 'uptime'
来源：http://hz.haohaochexian.top/gtlrtmukjq.html

[R58] 下载文件
来源：http://hz.yuanzhike.top/gtoznjtqdo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinqigfzy.top/gtrkrulvkj.html

[R59] 发 POST JSON
来源：http://hz.yanxiufei.cn/gtbegofxjv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinqigfzy.top/gtksuakvdf.html

[R60] 只看 HTTP 状态码
来源：http://hz.ppjwa.cn/gtztwxcycp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.316326.xyz/gtmftglonl.html

[R61] 磁盘占用
来源：http://hz.chenjidiqi.icu/gtukgbmcge.html

df -h;  du -sh *
来源：http://hz.c1oappe.top/gtqjlyxlhx.html

[R62] 找最占空间的文件
来源：http://hz.fengsongda.top/gtykruclso.html

du -ah . | sort -rh | head -10
来源：http://hz.xuanzx.com/gtqyddwchb.html

[R63] 内存与进程
来源：http://hz.nwbrower.top/gtvlaugozf.html

free -h;  ps aux | grep nginx
来源：http://hz.52xcode.cn/gtkvhvlqtq.html

[R64] 结束进程
来源：http://hz.hongshengwenyu.top/gtyqvgiurr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.aizwys.cn/gtrpceewrw.html

[R65] 查看端口占用
来源：http://hz.yangfankeji.com/gtqbbyvkhb.html


<!-- 参考信息 -->