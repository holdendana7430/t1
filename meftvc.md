代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xziqi.cn/gtydwzcorj.html

[Q18] 模糊匹配
来源：http://hz.gzhubu.top/gtcwaaauon.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cucudq.cn/gttqhbkmah.html

[Q19] 范围查询
来源：http://hz.hongshengwenyu.top/gtfqoayujt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jiagoushi.top/gttsfitnlt.html

[Q20] IN 列表
来源：http://hz.gaohongyu789.top/gtzzpamzlg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.snrcjt.cn/gtmeturvro.html

[Q21] 空值判断
来源：http://hz.0kj1m.cn/gtbiocblmb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gotoacloud.top/gtnxydzmss.html

[Q22] 排序
来源：http://hz.ppjwa.cn/gteqnoynjg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.andypj.xyz/gtmjxapikk.html

[Q23] 分页
来源：http://hz.andypj.xyz/gtcgufntgj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ybcxt.top/gtkafkaoue.html

[Q24] 去重
来源：http://hz.dashuyun.cn/gtuyoshjty.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj202588.top/gtijhrkwmn.html

[Q25] 只取前 N 条
来源：http://hz.jinyuanbaomall.cn/gtoeddteco.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.chenzaomai.com/gtqofigdxr.html

[Q26] 计数
来源：http://hz.shangyingyoupin.top/gttprzntxn.html

SELECT COUNT(*) FROM users;
来源：http://hz.yangfankeji.com/gtqrvqugwy.html

[Q27] 条件计数
来源：http://hz.bjfxy.top/gtdvjijbuo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cdnleiting.top/gtifuwpxfw.html

[Q28] 求和与平均
来源：http://hz.gaohongyu789.top/gtunvxoxyv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zdqjudy.top/gtazybuvra.html

[Q29] 最大最小值
来源：http://hz.gaohongyu789.top/gthekbdktf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.vqdsnc.cn/gtqgajkltt.html

[Q30] 分组统计
来源：http://hz.shangyingyoupin.top/gtyxnpawyk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtoflyzbgx.html

[Q31] 分组后过滤
来源：http://hz.yj20258.top/gtqwgkyesu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.c1oappe.top/gtdbwejhyv.html

[Q32] 分组拼接字符串
来源：http://hz.ehwqpu.com/gthqdgexnp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jianghu66.top/gtnptjeilk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.meibo888.top/gtxgkehqwo.html

[Q33] 多列分组
来源：http://hz.52xcode.cn/gtqjwevrhl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.iojbl.cn/gtbpigscev.html

[Q34] 每组取第一条
来源：http://hz.jinqigufen.top/gtpgbnnliu.html

SELECT * FROM (
来源：http://hz.c1oappe.top/gttoggdqxp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yuxming.cn/gtgtotgmjz.html

) t WHERE rn = 1;
来源：http://hz.yj202588.top/gtqdcguglt.html

[Q35] 内连接
来源：http://hz.vqdsnc.cn/gtrflaqmqo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuanzx.com/gtbzmuntju.html

[Q36] 左连接
来源：http://hz.hysaishi.cn/gtoqrdbweb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.guowangkeji.top/gtgcehsojm.html

[Q37] 右连接
来源：http://hz.sxryk.cn/gtgwttbulp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.daria6918.cn/gtebtealse.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yvedp.cn/gtrevkjrlc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.daria6918.cn/gtlypkbvbw.html

[Q39] 自连接（查上下级）
来源：http://hz.wangshuangyany.cn/gtnvolajlb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hfpthk.cn/gtubuemwez.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.fengsongda.top/gtropufwdi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.bjfxy.top/gtepnfjxoo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.c1oappe.top/gtoswfnkpk.html

[Q41] 多表连接
来源：http://hz.tianlin.xyz/gtauhumbwy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.dianchejie.cn/gtyejsnioc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.chenzaomai.com/gtzmbiigxl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.tian-w.cn/gtdiuyzeaq.html

[Q42] 连接条件附加过滤
来源：http://hz.jqgfzy.top/gtujlmgark.html

SELECT u.name, o.amount FROM users u
来源：http://hz.havefunace.top/gtpdommcyy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhongyouzk.top/gtgkihsyki.html

[Q43] 标量子查询
来源：http://hz.hywenlv.cn/gtqezuwxsz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xuanzx.com/gtrsxgzbuj.html

[Q44] IN 子查询
来源：http://hz.wangshuangyany.cn/gtpbrrahmg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.aibaodan.cn/gtwpewuvfi.html

[Q45] EXISTS 判断存在
来源：http://hz.hnqzz.top/gtiqnrbsox.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.mhx1999.top/gtruheyyvp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hnxiangtu.top/gttwrmhmyl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.svipenyu.cn/gtaxrlzhri.html

[Q47] 与平均值比较
来源：http://hz.zycfv.cn/gtwdvbylrt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nwbrower.top/gtuhdiiaji.html

[Q48] CTE 公用表表达式
来源：http://hz.316326.xyz/gtlbkxbiou.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yj20258888.top/gtdpdjaynk.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhaomingkeji.xyz/gtgeujzrru.html

[Q49] 更新单行
来源：http://hz.ywan-chungtsiang.top/gtnshvunko.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sufxvd.cn/gtqovqkfkb.html

[Q50] 批量更新
来源：http://hz.chenjidiqi.icu/gtsguavzjt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xingfuxueyuan.xyz/gtxaqtumpb.html

[Q51] 用子查询更新
来源：http://hz.wangshuangyany.cn/gtiqfqmvkc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xingfuxueyuan.xyz/gtrakeeqcx.html

[Q52] 删除指定行
来源：http://hz.sweek.top/gtkbedoezi.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hywenlv.cn/gtfddwcach.html

[Q53] 按条件删除
来源：http://hz.zhengqikj.top/gtilikmivd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nanxuanxn.top/gtslwtochw.html

[Q54] 清空表
来源：http://hz.sxryk.cn/gttrbeedgh.html

TRUNCATE TABLE logs;
来源：http://hz.jqgfzy.top/gtrtjdgbaf.html

[Q55] 排名（并列占位）
来源：http://hz.zdqjudy.top/gtuofbfrdd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hnxiangtu.top/gtydcojmhk.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hnxiangtu.top/gtozdualrf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhoulong.xyz/gtdalqolvg.html

[Q57] 行号
来源：http://hz.vqdsnc.cn/gttbolfyba.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hywenlv.cn/gtrcmbqtoq.html

[Q58] 累计求和
来源：http://hz.iojbl.cn/gtpfcohbxw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.feifeiyinyue.top/gtewvrupkv.html

[Q59] 分组内累计
来源：http://hz.zhongyouzk.top/gtyldatkcg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.svipenyu.cn/gtfkheknho.html

[Q60] 取上一行 / 下一行
来源：http://hz.ehwqpu.com/gtokvhtcxk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.svipenyu.cn/gtzrunbqzr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zycfv.cn/gtuiwennjm.html

[Q61] 移动平均
来源：http://hz.sxryk.cn/gtdoyzlmwm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.andypj.xyz/gtnugdvtqq.html

[Q62] 分组占比
来源：http://hz.mhx1999.top/gtzwqpxdna.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ydzc1.top/gtohdlnjrg.html

[Q63] 开启事务
来源：http://hz.ybcxt.top/gtgbnugxiy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhongyouzk.top/gtnsbvkomp.html

[Q64] 提交事务
来源：http://hz.smart0.xyz/gtqtwsyyko.html

COMMIT;
来源：http://hz.sxryk.cn/gtcvgmvldg.html

[Q65] 回滚事务
来源：http://hz.yj20258888.top/gtskocpxmq.html

ROLLBACK;
来源：http://hz.birdmap.top/gthxgqsybd.html

[Q66] 行锁查询
来源：http://hz.yj20258888.top/gtjghcwjbr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.316326.xyz/gtsbgefmpl.html

[Q67] 设置隔离级别
来源：http://hz.fengsongda.top/gtwcuhjidu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jqgufenzy.top/gtglmhchgu.html

[Q68] 保存点
来源：http://hz.chenzaomai.com/gtubavioax.html

SAVEPOINT sp1;
来源：http://hz.zhixingplan.top/gtryubaqfs.html

ROLLBACK TO sp1;
来源：http://hz.guannengcc.top/gtihkrjzud.html

[Q69] 查看执行计划
来源：http://hz.cucudq.cn/gtgxirpkvi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.vqdsnc.cn/gtrtaolwob.html

[Q70] 更新统计信息
来源：http://hz.yonumen.top/gtezaejobj.html

ANALYZE TABLE users;
来源：http://hz.pengpengdd.cyou/gtjjpolihw.html

[Q71] 查看建表语句
来源：http://hz.jinqigufen.top/gtcpbcqaee.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.dianchejie.cn/gtawlbpubo.html

[Q72] 查看索引
来源：http://hz.vqdsnc.cn/gtaiedffmu.html

SHOW INDEX FROM users;
来源：http://hz.yuxming.cn/gtkextuuci.html

[Q73] 查看表状态
来源：http://hz.zhoulong.xyz/gtszhurgif.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jqgfzy.top/gtgwubwxuj.html

[Q74] 强制使用索引
来源：http://hz.bjfxy.top/gtmpijrvxj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hnqzz.top/gtqbnotqnm.html

[Q75] 日期格式化
来源：http://hz.haohaochexian.top/gtehhewebr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtluvplzsg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.tianlin.xyz/gtxeoxpasy.html

[Q76] 按天统计
来源：http://hz.daria6918.cn/gtwsfxtcom.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tian-w.cn/gtpquzchuo.html

[Q77] 时间加减
来源：http://hz.kuanghao11.cn/gtillhurqt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zycfv.cn/gtoriffhdw.html

[Q78] 当前时间
来源：http://hz.sysykeji.top/gtsuifgecq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.snrcjt.cn/gtjjlxrnqw.html

[Q79] 字符串拼接
来源：http://hz.xylfe.cn/gtmbjdkopy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.pycfn.com/gthkdwiyib.html

[Q80] 字符串截取
来源：http://hz.hongshengwenyu.top/gtvfmmkqfg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ydzc1.top/gtibmsarrn.html

[Q81] 字符串替换
来源：http://hz.cashguo.top/gtjywnfdlv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.pycfn.com/gtzukeybkb.html

[Q82] 字符长度与字节长度
来源：http://hz.daxiang520.top/gtbktyljyd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtkjdsalge.html

[Q83] 大小写转换
来源：http://hz.daxiang520.top/gtmeshjblh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sxryk.cn/gtyencipyu.html

[Q84] 去除首尾空格
来源：http://hz.tianlin.xyz/gtickkktxn.html

SELECT TRIM(name) FROM users;
来源：http://hz.yanxiufei.cn/gthcluhmgn.html

[Q85] 数值取整
来源：http://hz.jlsjyb.cn/gtynrjykkg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.chenjidiqi.icu/gtcvglglrt.html

[Q86] 读取 JSON 字段
来源：http://hz.hnxiangtu.top/gttbikgoro.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yueranfly.top/gtgvwqqzgp.html

[Q87] JSON 字段做条件
来源：http://hz.gzhubu.top/gthwukmeyt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.fengsongda.top/gtqglgdssj.html

[Q88] 行转列（条件聚合）
来源：http://hz.shanyushiyangkeji.top/gtibtaiwrc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gotoacloud.top/gtfqfzcfhn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jlsjyb.cn/gtjwpkguyr.html

[Q89] 判断表是否存在
来源：http://hz.yuanzhike.top/gtfjasfdoc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zdqjudy.top/gtiznpfwsk.html

[Q90] 生成序号列
来源：http://hz.guowangkeji.top/gtessiuqmb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.aizwys.cn/gtekypyvua.html

================================================================================
来源：http://hz.zhijiandao.cn/gtffivlswp.html

R. Bash 专题
来源：http://hz.vqdsnc.cn/gtvrgighph.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtxwhxgotv.html

[R01] shebang 与严格模式
来源：http://hz.gogol.net.cn/gtrqxwfxoa.html

#!/usr/bin/env bash
来源：http://hz.nanxinkj.top/gtitvivgbz.html

set -euo pipefail
来源：http://hz.gotoacloud.top/gtilwlniop.html

[R02] 变量赋值与使用
来源：http://hz.yanxiufei.cn/gtmeqiabrk.html

name="Tom"; echo "$name"
来源：http://hz.ydjk.org.cn/gtnzglyfef.html

[R03] 只读变量
来源：http://hz.dianchejie.cn/gtpyhpvzxu.html

readonly PI=3.14
来源：http://hz.sufxvd.cn/gthtgnaxmn.html

[R04] 位置参数
来源：http://hz.316326.xyz/gtfvkdqpbw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.snrcjt.cn/gtvdeqdyih.html

[R05] 参数默认值
来源：http://hz.xylfe.cn/gtfiqumzym.html

name="${1:-default}"
来源：http://hz.daxiang520.top/gtfwzhawtk.html

[R06] 判断命令是否存在
来源：http://hz.ydzc1.top/gtzbbozupi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cashguo.top/gtuzpedrpg.html

[R07] if 判断文件
来源：http://hz.haohaochexian.top/gtdpyhjwfn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.wangdashe.top/gtdkhcnlqp.html

[R08] 数值比较
来源：http://hz.birdmap.top/gtklikukrz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.feifeiyinyue.top/gtmimjifqf.html

[R09] 字符串比较
来源：http://hz.zdqjudy.top/gtqngotibe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tanke756.top/gteqqeabeb.html

[R10] 正则匹配
来源：http://hz.cqqwz.cn/gtbjvtpxwh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zycfv.cn/gtmzmsptlg.html

[R11] case 多分支
来源：http://hz.havefunace.top/gtrpitkdwc.html

case "$1" in
来源：http://hz.zhaomingkeji.xyz/gtkjxehdvy.html

start) echo "启动" ;;
来源：http://hz.xinyue.icu/gtbghutnza.html

stop)  echo "停止" ;;
来源：http://hz.ivvv.top/gtxpxxaisz.html

*)     echo "未知命令" ;;
来源：http://hz.chenjidiqi.icu/gtdrutucly.html

esac
来源：http://hz.aizwys.cn/gtjimylnyy.html

[R12] for 遍历文件
来源：http://hz.xylfe.cn/gteuzfolsm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ywan-chungtsiang.top/gtsgbkbkss.html

[R13] for 计数循环
来源：http://hz.yj20258.top/gtgvuootms.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yueranfly.top/gtdvliuezb.html

[R14] C 风格 for
来源：http://hz.kuanghao11.cn/gtvpvncypv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinqigfzy.top/gtrojscxhz.html

[R15] while 逐行读文件
来源：http://hz.bjfxy.top/gtygcuyhmf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.wangdashe.top/gtbveawwfp.html

[R16] until 等待条件
来源：http://hz.shanyushiyangtech.top/gtjuphzjuz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zdqjudy.top/gtuboqmrla.html

[R17] 数组定义与取值
来源：http://hz.shuidangran.top/gtdbmjkobt.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hnqzz.top/gtyucynvuy.html

[R18] 遍历数组
来源：http://hz.zdqjudy.top/gtxrnufwyr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.chenjidiqi.icu/gtslprrfji.html

[R19] 数组长度
来源：http://hz.zhijiandao.cn/gtfhznzezc.html

echo "${#arr[@]}"
来源：http://hz.hammf.cn/gtnvncuesc.html

[R20] 关联数组（字典）
来源：http://hz.hongshengwenyu.top/gtjvjykoeh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zdqjudy.top/gtubrojfqr.html

[R21] 字符串长度
来源：http://hz.iojbl.cn/gtvmzigwpz.html

echo "${#s}"
来源：http://hz.chenlongwang.top/gtmwihwypo.html

[R22] 截取子串
来源：http://hz.hywenlv.cn/gtqewxoagq.html

echo "${s:0:5}"
来源：http://hz.cheryme.top/gtmupgnuqe.html

[R23] 字符串替换
来源：http://hz.cdnleiting.top/gtdxhmidrv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinyuanbaomall.cn/gtewutbpkf.html

[R24] 大小写转换
来源：http://hz.jqgufenzy.top/gthkkccyha.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cheryme.top/gtgrtpwefs.html

[R25] 去后缀 / 去前缀
来源：http://hz.0kj1m.cn/gtccsydyuz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.vqdsnc.cn/gtlsbsfxow.html

[R26] 命令替换
来源：http://hz.jinqigfzy.top/gtuvghetmc.html

now=$(date +%F); echo "$now"
来源：http://hz.0kj1m.cn/gtatdieptu.html

[R27] 算术展开
来源：http://hz.yvedp.cn/gtbltaydzy.html

echo $((1 + 2 * 3))
来源：http://hz.sweek.top/gtcnqsfohm.html

[R28] 浮点运算
来源：http://hz.xuanzx.com/gtgvviaapt.html

echo "scale=2; 10/3" | bc
来源：http://hz.aizwys.cn/gttqzkvjgi.html

[R29] 定义函数
来源：http://hz.meibo888.top/gtesuzblbv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shanyushiyangkeji.top/gteausaplw.html

[R30] 函数返回状态码
来源：http://hz.gzhubu.top/gtbykwjsev.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.havefunace.top/gtlotysspo.html

[R31] 局部变量
来源：http://hz.yj20258.top/gtefbxvszh.html

f() { local x=1; echo "$x"; }
来源：http://hz.ehwqpu.com/gtccuqkmnu.html

[R32] 参数个数校验
来源：http://hz.jinyuanbaomall.cn/gtrrjlpslm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinyuanbaomall.cn/gtrwhpihvx.html

[R33] 捕获错误并提示行号
来源：http://hz.chenzaomai.com/gtrmbfthjd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.9152youxi.cn/gtlqnyhcri.html

[R34] 退出时清理
来源：http://hz.jinyuanbaomall.cn/gtefxxoweh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shuidangran.top/gtkdtjndrf.html

[R35] 后台执行并等待
来源：http://hz.ppjwa.cn/gtokdzcdeq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hywenlv.cn/gtruguhivq.html

[R36] 并发执行多个任务
来源：http://hz.havefunace.top/gtclzygcmn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhaomingkeji.xyz/gtqubkdlbr.html

[R37] 把输出赋给变量
来源：http://hz.yj20258888.top/gtltlpvdcp.html

files=$(ls -1)
来源：http://hz.tanke756.top/gtsguamdpx.html

[R38] 管道串联
来源：http://hz.sweek.top/gtptvbbhmj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jiagoushi.top/gtsjecxbxl.html

[R39] 重定向标准输出与错误
来源：http://hz.zdqjudy.top/gtbkrvosbm.html

cmd > out.log 2>&1
来源：http://hz.vqdsnc.cn/gtvpqifzqj.html

[R40] 追加写日志
来源：http://hz.aizwys.cn/gtzuqwjwoo.html

echo "log" >> out.log
来源：http://hz.gaohongyu789.top/gtvftnxnsu.html

[R41] 丢弃输出
来源：http://hz.yangfankeji.com/gtqgijjlhm.html

cmd >/dev/null 2>&1
来源：http://hz.gotoacloud.top/gtpmborphr.html

[R42] 输入重定向
来源：http://hz.dashuyun.cn/gtgsozsyqf.html

wc -l < a.txt
来源：http://hz.svipenyu.cn/gtiifpaxjx.html

[R43] 按名字查找文件
来源：http://hz.ehwqpu.com/gtuipdsgyx.html

find . -name "*.log" -type f
来源：http://hz.hammf.cn/gtcymabcui.html

[R44] 按修改时间查找
来源：http://hz.xingfuxueyuan.xyz/gtrsbqnlfg.html

find . -mtime -7 -type f
来源：http://hz.xinyue.icu/gtnvqmqshy.html

[R45] 批量删除
来源：http://hz.jiagoushi.top/gtjrvppgyr.html

find . -name "*.tmp" -delete
来源：http://hz.xinyue.icu/gtccaluzmt.html

[R46] 递归替换文件内容
来源：http://hz.yj20258888.top/gtdfncvtfb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xingfuxueyuan.xyz/gtzoucybdv.html

[R47] sed 单行替换
来源：http://hz.yj20258888.top/gtktbcvkaw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.vqdsnc.cn/gtiqfzmbtj.html

[R48] awk 取指定列
来源：http://hz.ywan-chungtsiang.top/gtvpmolcdu.html

awk '{print $1, $3}' a.txt
来源：http://hz.ehwqpu.com/gtmebiqhyx.html

[R49] awk 带条件
来源：http://hz.xinyue.icu/gtcqzscaqh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.guowangkeji.top/gtppdmrdjo.html

[R50] awk 求和
来源：http://hz.nanxuanxn.top/gttnkflrto.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hysaishi.cn/gtjizrqogs.html

[R51] 排序去重取前几
来源：http://hz.aibaodan.cn/gthtlxnjfw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shanyushiyangkeji.top/gtnltiqfke.html

[R52] 统计行数
来源：http://hz.ydzc1.top/gtlndlwnoq.html

wc -l a.txt
来源：http://hz.yj20258.top/gtarifbljz.html

[R53] 查看文件头与实时尾
来源：http://hz.0kj1m.cn/gtzoqoasxz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cdnleiting.top/gtoktuaopf.html

[R54] 比较两个文件
来源：http://hz.jyoumei.cn/gtsnbjzrcd.html

diff a.txt b.txt
来源：http://hz.c1oappe.top/gtkihmiuwg.html

[R55] 压缩与解压
来源：http://hz.xziqi.cn/gtvdbrlyuu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yangfankeji.com/gtlkifbebs.html

[R56] 远程拷贝
来源：http://hz.hammf.cn/gtdhqrduvk.html

scp file user@host:/path/
来源：http://hz.chenzaomai.com/gtzsqfavtz.html

[R57] 远程执行命令
来源：http://hz.jqgfzy.top/gthuvwwqfe.html

ssh user@host 'uptime'
来源：http://hz.pengpengdd.cyou/gtkitdtagu.html

[R58] 下载文件
来源：http://hz.9152youxi.cn/gtetjaewye.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.dashuyun.cn/gtiwgftbwx.html

[R59] 发 POST JSON
来源：http://hz.9152youxi.cn/gtneanzuwg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.andypj.xyz/gtkwdvnvyx.html

[R60] 只看 HTTP 状态码
来源：http://hz.cdnleiting.top/gtutbnndmf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yueranfly.top/gtphzvbaly.html

[R61] 磁盘占用
来源：http://hz.52xcode.cn/gtjfpqlyeb.html

df -h;  du -sh *
来源：http://hz.zhijiandao.cn/gtofhgoybw.html

[R62] 找最占空间的文件
来源：http://hz.xziqi.cn/gtwaachnkh.html

du -ah . | sort -rh | head -10
来源：http://hz.aizwys.cn/gtuwjkhdvi.html

[R63] 内存与进程
来源：http://hz.feifeiyinyue.top/gtqafaexsr.html

free -h;  ps aux | grep nginx
来源：http://hz.chenjidiqi.icu/gtvraulsot.html

[R64] 结束进程
来源：http://hz.gogol.net.cn/gtbthwcntj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigfzy.top/gtussiqqqu.html

[R65] 查看端口占用
来源：http://hz.aizwys.cn/gtnqhtzudu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yangfankeji.com/gtyensuine.html

[R66] 定时任务
来源：http://hz.mhx1999.top/gtteecjtki.html

crontab -e;  crontab -l
来源：http://hz.gaohongyu789.top/gtayzyjvsu.html

[R67] 生成随机十六进制串
来源：http://hz.sufxvd.cn/gtdjudylpb.html


<!-- 参考信息 -->