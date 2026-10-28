代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.c1oappe.top/gtgqbpyvjn.html

[Q24] 去重
来源：http://hz.yueranfly.top/gtzukmkeyf.html

SELECT DISTINCT city FROM users;
来源：http://hz.yanxiufei.cn/gtyzbmusso.html

[Q25] 只取前 N 条
来源：http://hz.bjfxy.top/gtjxsylajh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cucudq.cn/gtlimxtolp.html

[Q26] 计数
来源：http://hz.zhijiandao.cn/gtdwomrbmq.html

SELECT COUNT(*) FROM users;
来源：http://hz.sysykeji.top/gtulxkpmku.html

[Q27] 条件计数
来源：http://hz.nanxinkj.top/gtswexlbfb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shanyushiyangkeji.top/gtccywhwau.html

[Q28] 求和与平均
来源：http://hz.fengsongda.top/gtrwobphst.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.nwbrower.top/gtifcowyzn.html

[Q29] 最大最小值
来源：http://hz.xuanzx.com/gtisrvhjcn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shzxlz.cn/gtrwgoqedi.html

[Q30] 分组统计
来源：http://hz.feifeiyinyue.top/gtkgcrmuek.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yuanzhike.top/gtxpzavtap.html

[Q31] 分组后过滤
来源：http://hz.zhoulong.xyz/gtyhjaujtd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinqigufen.top/gthjgknabv.html

[Q32] 分组拼接字符串
来源：http://hz.yuxming.cn/gttlejwpxl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtxmxmesdn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hnxiangtu.top/gteufhnyyr.html

[Q33] 多列分组
来源：http://hz.sufxvd.cn/gtkdomaffb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daria6918.cn/gtmitboxon.html

[Q34] 每组取第一条
来源：http://hz.jiagoushi.top/gtawsdcqjx.html

SELECT * FROM (
来源：http://hz.dianchejie.cn/gthyinemvx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.mhx1999.top/gtrlhzvzcj.html

) t WHERE rn = 1;
来源：http://hz.aibaodan.cn/gtxkhfjdsj.html

[Q35] 内连接
来源：http://hz.nanxuanxn.top/gtxcpucbxa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258888.top/gtlfzeeqah.html

[Q36] 左连接
来源：http://hz.aibaodan.cn/gtfivruiqv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnxiangtu.top/gtibkhwwct.html

[Q37] 右连接
来源：http://hz.zhixingplan.top/gtqtmxcwcm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xinyue.icu/gtbjaahsqt.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fengsongda.top/gtizropine.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gaohongyu789.top/gtvejwhjke.html

[Q39] 自连接（查上下级）
来源：http://hz.kuanghao11.cn/gttcqmnlxb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.52xcode.cn/gtnqkuagoz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shzxlz.cn/gtlezexpng.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenlongwang.top/gtafsbzhok.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zycfv.cn/gtzescyvng.html

[Q41] 多表连接
来源：http://hz.52xcode.cn/gtzwnwdoqs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ivvv.top/gtvdqukrvs.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhiwuduotai.top/gtpudzjwfs.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xinyue.icu/gtdterkmqt.html

[Q42] 连接条件附加过滤
来源：http://hz.zhongyouzk.top/gtzuszjzkl.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinyuanbaomall.cn/gtkzvrfoct.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ybcxt.top/gtbpgfmdrj.html

[Q43] 标量子查询
来源：http://hz.sxryk.cn/gtdsxjnxin.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.c1oappe.top/gtkbquweho.html

[Q44] IN 子查询
来源：http://hz.daxiang520.top/gtndntokis.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.52xcode.cn/gtdtbctqzb.html

[Q45] EXISTS 判断存在
来源：http://hz.tianlin.xyz/gtgjiehtwr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xziqi.cn/gtoppgfjdz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hysaishi.cn/gtvbkvrhdb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gtxebqvewk.html

[Q47] 与平均值比较
来源：http://hz.ybcxt.top/gtfqkqhtfj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cdnleiting.top/gtvjsgqssc.html

[Q48] CTE 公用表表达式
来源：http://hz.316326.xyz/gtgusrogst.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tanke756.top/gtsdtxtpqz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinqigfzy.top/gtthubuthw.html

[Q49] 更新单行
来源：http://hz.cashguo.top/gtrbluhseh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.52xcode.cn/gtgowslfdm.html

[Q50] 批量更新
来源：http://hz.shanyushiyangkeji.top/gtvmvdvtpq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shanyushiyangkeji.top/gtxeswyltr.html

[Q51] 用子查询更新
来源：http://hz.zycfv.cn/gtoxqxfncs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yuanzhike.top/gtilqdbixm.html

[Q52] 删除指定行
来源：http://hz.yj20258888.top/gtxticymzh.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xinyue.icu/gtylmmebyt.html

[Q53] 按条件删除
来源：http://hz.52xcode.cn/gtuomyiqgo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gzhubu.top/gtgzilfdjf.html

[Q54] 清空表
来源：http://hz.sweek.top/gtblhfcpuk.html

TRUNCATE TABLE logs;
来源：http://hz.ehwqpu.com/gtbrrldsfb.html

[Q55] 排名（并列占位）
来源：http://hz.zhaomingkeji.xyz/gtcpvnkjrx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhongyouzk.top/gtwihwkcxc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ydjk.org.cn/gtkyvtskqk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hywenlv.cn/gtzvhwstph.html

[Q57] 行号
来源：http://hz.ivvv.top/gtjmupuhrj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gzhubu.top/gtkvmqmnsu.html

[Q58] 累计求和
来源：http://hz.ywan-chungtsiang.top/gtjedyvqqq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinghuilouyu.cn/gtzemylhle.html

[Q59] 分组内累计
来源：http://hz.iojbl.cn/gtqzoxwppo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zycfv.cn/gtiobxtctt.html

[Q60] 取上一行 / 下一行
来源：http://hz.0kj1m.cn/gtewkpfxwk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.dashuyun.cn/gtogdeuvez.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.aibaodan.cn/gtlsxjjzya.html

[Q61] 移动平均
来源：http://hz.mhx1999.top/gtavrhebzm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.tanke756.top/gtwhrumgej.html

[Q62] 分组占比
来源：http://hz.jlsjyb.cn/gtgebgijdi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.smart0.xyz/gtpptuglbk.html

[Q63] 开启事务
来源：http://hz.fengsongda.top/gtsftcvkes.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yuanzhike.top/gtyoqmzoie.html

[Q64] 提交事务
来源：http://hz.ppjwa.cn/gtuqdutmbw.html

COMMIT;
来源：http://hz.jianghu66.top/gtywdaoygv.html

[Q65] 回滚事务
来源：http://hz.yangfankeji.com/gtidsenabg.html

ROLLBACK;
来源：http://hz.jinqigfzy.top/gtactarokt.html

[Q66] 行锁查询
来源：http://hz.aibaodan.cn/gthefnlosx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.andypj.xyz/gtjrsxsbob.html

[Q67] 设置隔离级别
来源：http://hz.jqgfzy.top/gtfqhobner.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yonumen.top/gtlteyruti.html

[Q68] 保存点
来源：http://hz.nanxinkj.top/gtsbenxqsm.html

SAVEPOINT sp1;
来源：http://hz.wangshuangyany.cn/gtkehgjzro.html

ROLLBACK TO sp1;
来源：http://hz.yanxiufei.cn/gteaiwqqyd.html

[Q69] 查看执行计划
来源：http://hz.jqgfzy.top/gtwqccluga.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hysaishi.cn/gthvnqswxq.html

[Q70] 更新统计信息
来源：http://hz.52xcode.cn/gtajnpzixc.html

ANALYZE TABLE users;
来源：http://hz.gzhubu.top/gtbonkdaqt.html

[Q71] 查看建表语句
来源：http://hz.tianlin.xyz/gtlaweurta.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hongshengwenyu.top/gtdzqglmkn.html

[Q72] 查看索引
来源：http://hz.hysaishi.cn/gtethiuidy.html

SHOW INDEX FROM users;
来源：http://hz.quarkkingdee.top/gtlzksxwiy.html

[Q73] 查看表状态
来源：http://hz.daria6918.cn/gtujceeixt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.52xcode.cn/gtagxbdpmn.html

[Q74] 强制使用索引
来源：http://hz.wangshuangyany.cn/gtxhfkhhuy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jianghu66.top/gtdbtnubsx.html

[Q75] 日期格式化
来源：http://hz.tanke756.top/gttkrklorn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.tanke756.top/gtlypilyhu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yanxiufei.cn/gtstegbnqo.html

[Q76] 按天统计
来源：http://hz.hywenlv.cn/gtrarztbhe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hnqzz.top/gtzgcypdjm.html

[Q77] 时间加减
来源：http://hz.pengpengdd.cyou/gtxtywdeev.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.redwolf501.top/gtaizzejzi.html

[Q78] 当前时间
来源：http://hz.gogol.net.cn/gtwontellj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hywenlv.cn/gtqudimyad.html

[Q79] 字符串拼接
来源：http://hz.daria6918.cn/gtjkmemlgg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.fzhhl.top/gtzewlsjsp.html

[Q80] 字符串截取
来源：http://hz.jinyuanbaomall.cn/gteerripuu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sufxvd.cn/gtscsunncu.html

[Q81] 字符串替换
来源：http://hz.gaohongyu789.top/gtirwhzcxw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.aibaodan.cn/gtnaizeqwg.html

[Q82] 字符长度与字节长度
来源：http://hz.shanyushiyangkeji.top/gtvxmrnwcw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yangfankeji.com/gtvnhaspnt.html

[Q83] 大小写转换
来源：http://hz.hywenlv.cn/gtcahmydug.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinqigufen.top/gtjhihfvln.html

[Q84] 去除首尾空格
来源：http://hz.cheryme.top/gtnbbicqgh.html

SELECT TRIM(name) FROM users;
来源：http://hz.0kj1m.cn/gtydberraj.html

[Q85] 数值取整
来源：http://hz.daria6918.cn/gtqedhzwdd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cucudq.cn/gtofmptxxx.html

[Q86] 读取 JSON 字段
来源：http://hz.snrcjt.cn/gtnrpdymdn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gogol.net.cn/gtkyvagysw.html

[Q87] JSON 字段做条件
来源：http://hz.sysykeji.top/gtkpkargog.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jlsjyb.cn/gtwcdjzuak.html

[Q88] 行转列（条件聚合）
来源：http://hz.vqdsnc.cn/gtxxhvemub.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yueranfly.top/gthvpochdb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cucudq.cn/gtdwmwqitw.html

[Q89] 判断表是否存在
来源：http://hz.ydzc1.top/gtvgdbnpkt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinqigufen.top/gtqybndows.html

[Q90] 生成序号列
来源：http://hz.chenjidiqi.icu/gtlzdgkisf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.wangshuangyany.cn/gtuuafeygm.html

================================================================================
来源：http://hz.aibaodan.cn/gtztagkrlq.html

R. Bash 专题
来源：http://hz.zhongyouzk.top/gtvbtfcinh.html

================================================================================
来源：http://hz.daxiang520.top/gtkoedljnv.html

[R01] shebang 与严格模式
来源：http://hz.shangyingyoupin.top/gtrbuniqxy.html

#!/usr/bin/env bash
来源：http://hz.sweek.top/gtrhipnppt.html

set -euo pipefail
来源：http://hz.shzxlz.cn/gtgkjtnumn.html

[R02] 变量赋值与使用
来源：http://hz.yj20258888.top/gttpbnkcco.html

name="Tom"; echo "$name"
来源：http://hz.xuanzx.com/gtrmqvyxfv.html

[R03] 只读变量
来源：http://hz.52xcode.cn/gtfuiaeaix.html

readonly PI=3.14
来源：http://hz.yj20258888.top/gtdyrtmnry.html

[R04] 位置参数
来源：http://hz.cheryme.top/gtjfcuhjpl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhaomingkeji.xyz/gtzkadvagj.html

[R05] 参数默认值
来源：http://hz.fengsongda.top/gtfxkqieak.html

name="${1:-default}"
来源：http://hz.nanxuanxn.top/gtwsxiejva.html

[R06] 判断命令是否存在
来源：http://hz.ydjk.org.cn/gtmcnzpplt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.vqdsnc.cn/gtovkbzawo.html

[R07] if 判断文件
来源：http://hz.yonumen.top/gtyczqqdka.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj20258888.top/gtzniijsxf.html

[R08] 数值比较
来源：http://hz.fzhhl.top/gtomgkkrxb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tanke756.top/gtdwxyjgnf.html

[R09] 字符串比较
来源：http://hz.cqqwz.cn/gtwbdcqbjv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shuidangran.top/gtnwmcssso.html

[R10] 正则匹配
来源：http://hz.yj202588.top/gtyulrrvjk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhengqikj.top/gtoxwzvkwj.html

[R11] case 多分支
来源：http://hz.zhaomingkeji.xyz/gtxeyrvvvo.html

case "$1" in
来源：http://hz.gogol.net.cn/gtsknfqary.html

start) echo "启动" ;;
来源：http://hz.chenzaomai.com/gtobuvjxyy.html

stop)  echo "停止" ;;
来源：http://hz.yongpay.top/gtddhbjknx.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangtech.top/gtkddvyhpq.html

esac
来源：http://hz.0kj1m.cn/gtggvuaznx.html

[R12] for 遍历文件
来源：http://hz.gogol.net.cn/gtkapzenet.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenlongwang.top/gtsxkmkuqe.html

[R13] for 计数循环
来源：http://hz.sweek.top/gtmvgbtchv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenjidiqi.icu/gtvjnklimp.html

[R14] C 风格 for
来源：http://hz.yonumen.top/gtxztaomid.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.chenjidiqi.icu/gtvaosmjal.html

[R15] while 逐行读文件
来源：http://hz.aizwys.cn/gthshjlwvd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.smart0.xyz/gtdchjlmne.html

[R16] until 等待条件
来源：http://hz.ydzc1.top/gtyxaajrso.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.c1oappe.top/gtdxvxshwp.html

[R17] 数组定义与取值
来源：http://hz.ehwqpu.com/gtklxfeslz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zycfv.cn/gtftvfcuul.html

[R18] 遍历数组
来源：http://hz.c1oappe.top/gtifjctugl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.dashuyun.cn/gtgrxrebqv.html

[R19] 数组长度
来源：http://hz.0kj1m.cn/gtrqldoudo.html

echo "${#arr[@]}"
来源：http://hz.hywenlv.cn/gtdhbxykhu.html

[R20] 关联数组（字典）
来源：http://hz.zhaomingkeji.xyz/gtnyhpbdut.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.kuanghao11.cn/gtaahisnmw.html

[R21] 字符串长度
来源：http://hz.daxiang520.top/gtcecxarvr.html

echo "${#s}"
来源：http://hz.ydjk.org.cn/gtqlttyhup.html

[R22] 截取子串
来源：http://hz.kuanghao11.cn/gtkjkjlunz.html

echo "${s:0:5}"
来源：http://hz.iojbl.cn/gtpplhvath.html

[R23] 字符串替换
来源：http://hz.hywenlv.cn/gtwnuvcpxr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ywan-chungtsiang.top/gtodpptffs.html

[R24] 大小写转换
来源：http://hz.zhongyouzk.top/gtdkxrrzly.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ybcxt.top/gtydvsvxmf.html

[R25] 去后缀 / 去前缀
来源：http://hz.jianghu66.top/gtpapdhzmg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhijiandao.cn/gtrcnrnltc.html

[R26] 命令替换
来源：http://hz.zhixingplan.top/gtmcdhffsh.html

now=$(date +%F); echo "$now"
来源：http://hz.xinyue.icu/gtgqbhxotf.html

[R27] 算术展开
来源：http://hz.yuanzhike.top/gtwgglsfgw.html

echo $((1 + 2 * 3))
来源：http://hz.daria6918.cn/gthfvdbsau.html

[R28] 浮点运算
来源：http://hz.hnxiangtu.top/gtkgvidnns.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenjidiqi.icu/gthddcxgzg.html

[R29] 定义函数
来源：http://hz.yj202588.top/gtzkflskep.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.pengpengdd.cyou/gtupekfbhw.html

[R30] 函数返回状态码
来源：http://hz.hnxiangtu.top/gthqjrzuub.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.svipenyu.cn/gthfjguhts.html

[R31] 局部变量
来源：http://hz.yuxming.cn/gtpvseismf.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhiwuduotai.top/gtwcmxkqqj.html

[R32] 参数个数校验
来源：http://hz.yangfankeji.com/gtkgxchmsu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.316326.xyz/gtwfoyifnr.html

[R33] 捕获错误并提示行号
来源：http://hz.xuetiantiany.cn/gtocxrfgzp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ehwqpu.com/gtuefuektt.html

[R34] 退出时清理
来源：http://hz.jianghu66.top/gtuiaqxive.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhixingplan.top/gtggdirvov.html

[R35] 后台执行并等待
来源：http://hz.yonumen.top/gtifyryitf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.aizwys.cn/gtdkkjlthp.html

[R36] 并发执行多个任务
来源：http://hz.c1oappe.top/gtoupvtvkw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.316326.xyz/gtjzyixlyw.html

[R37] 把输出赋给变量
来源：http://hz.sysykeji.top/gtnttozthl.html

files=$(ls -1)
来源：http://hz.cqqwz.cn/gtpnmdtymx.html

[R38] 管道串联
来源：http://hz.zhaomingkeji.xyz/gthjsfqvda.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yangfankeji.com/gteqnxnwpp.html

[R39] 重定向标准输出与错误
来源：http://hz.tianlin.xyz/gtwkexzaiz.html

cmd > out.log 2>&1
来源：http://hz.jqgufenzy.top/gtqjprkebk.html

[R40] 追加写日志
来源：http://hz.jlsjyb.cn/gtbekxonvy.html

echo "log" >> out.log
来源：http://hz.hammf.cn/gteuxgeqzm.html

[R41] 丢弃输出
来源：http://hz.xylfe.cn/gtvcxfkpai.html

cmd >/dev/null 2>&1
来源：http://hz.havefunace.top/gtwuzqhnnt.html

[R42] 输入重定向
来源：http://hz.sysykeji.top/gtqptcswrq.html

wc -l < a.txt
来源：http://hz.yj20258888.top/gthycahlzh.html

[R43] 按名字查找文件
来源：http://hz.ywan-chungtsiang.top/gtptgejdqo.html

find . -name "*.log" -type f
来源：http://hz.ybcxt.top/gtwzpkjkdn.html

[R44] 按修改时间查找
来源：http://hz.hywenlv.cn/gtxexhprjn.html

find . -mtime -7 -type f
来源：http://hz.chenjidiqi.icu/gtjdwsxkbn.html

[R45] 批量删除
来源：http://hz.cucudq.cn/gtntfyabsy.html

find . -name "*.tmp" -delete
来源：http://hz.sysykeji.top/gtrabeqjcf.html

[R46] 递归替换文件内容
来源：http://hz.yj20258.top/gtfuufshnh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.52xcode.cn/gtvggmscpy.html

[R47] sed 单行替换
来源：http://hz.shzxlz.cn/gtjaoimequ.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hongshengwenyu.top/gtbkvnfetm.html

[R48] awk 取指定列
来源：http://hz.feifeiyinyue.top/gtdmymldnv.html

awk '{print $1, $3}' a.txt
来源：http://hz.nanxinkj.top/gtqtswqgcv.html

[R49] awk 带条件
来源：http://hz.tianlin.xyz/gtnhugyveg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.guannengcc.top/gtusbqycod.html

[R50] awk 求和
来源：http://hz.jlsjyb.cn/gtgvpmnigc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gzhubu.top/gtvicndqmy.html

[R51] 排序去重取前几
来源：http://hz.fzhhl.top/gtnkwdiadq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.dianchejie.cn/gtfpfletad.html

[R52] 统计行数
来源：http://hz.nanxuanxn.top/gttytkhyvw.html

wc -l a.txt
来源：http://hz.chenlongwang.top/gtstbupfuv.html

[R53] 查看文件头与实时尾
来源：http://hz.shangyingyoupin.top/gtyqpoljvs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.mhx1999.top/gtegcgfkkb.html

[R54] 比较两个文件
来源：http://hz.gaohongyu789.top/gtxhbqchiq.html

diff a.txt b.txt
来源：http://hz.ppjwa.cn/gtbanobrqv.html

[R55] 压缩与解压
来源：http://hz.svipenyu.cn/gtrocefxag.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xingfuxueyuan.xyz/gttjmtrwfk.html

[R56] 远程拷贝
来源：http://hz.birdmap.top/gtcxeaceri.html

scp file user@host:/path/
来源：http://hz.pycfn.com/gtfeavwvom.html

[R57] 远程执行命令
来源：http://hz.ybcxt.top/gtlwdncdgl.html

ssh user@host 'uptime'
来源：http://hz.feifeiyinyue.top/gtplloyqzn.html

[R58] 下载文件
来源：http://hz.shanyushiyangkeji.top/gtopsdudpc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.daxiang520.top/gtyepyhxqc.html

[R59] 发 POST JSON
来源：http://hz.hnqzz.top/gtquoaoyvw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gogol.net.cn/gtnfuogidq.html

[R60] 只看 HTTP 状态码
来源：http://hz.xylfe.cn/gttrvxlylw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhiwuduotai.top/gttecnwcdd.html

[R61] 磁盘占用
来源：http://hz.mhx1999.top/gtmjxcejxd.html

df -h;  du -sh *
来源：http://hz.shanyushiyangtech.top/gtzrbzwmia.html

[R62] 找最占空间的文件
来源：http://hz.jyoumei.cn/gtqskbjznh.html

du -ah . | sort -rh | head -10
来源：http://hz.jinyuanbaomall.cn/gtmdabikgg.html

[R63] 内存与进程
来源：http://hz.gzhubu.top/gtldlfenhq.html

free -h;  ps aux | grep nginx
来源：http://hz.jinyuanbaomall.cn/gtyupltrye.html

[R64] 结束进程
来源：http://hz.ydzc1.top/gtxjfoaccm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sxryk.cn/gthypueyms.html

[R65] 查看端口占用
来源：http://hz.jyoumei.cn/gtdqcbxyos.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shuidangran.top/gtuukmrkff.html

[R66] 定时任务
来源：http://hz.shanyushiyangtech.top/gtoqnhaeun.html

crontab -e;  crontab -l
来源：http://hz.mhx1999.top/gtjitoawwf.html

[R67] 生成随机十六进制串
来源：http://hz.dianchejie.cn/gtdxlkvozj.html

openssl rand -hex 16
来源：http://hz.nanxuanxn.top/gtcufahtrw.html

[R68] 计算文件校验值
来源：http://hz.jyoumei.cn/gtnrxtdzwc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.tanke756.top/gtpxvokxgi.html

[R69] 生成随机密码
来源：http://hz.c1oappe.top/gtdkduszgt.html

head -c 16 /dev/urandom | base64
来源：http://hz.c1oappe.top/gtttnihezj.html

[R70] 时间戳与互转
来源：http://hz.fengsongda.top/gtqihqfffc.html

date +%s;  date -d @1700000000
来源：http://hz.shzxlz.cn/gtkingkneb.html

[R71] 日期格式化
来源：http://hz.hammf.cn/gtcdsjxbre.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jyoumei.cn/gtoufscafc.html

[R72] 等待端口就绪
来源：http://hz.zhixingplan.top/gtbwtbduir.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhengqikj.top/gttliqrgft.html

[R73] 分割大日志
来源：http://hz.zdqjudy.top/gtuzlhalwt.html


<!-- 参考信息 -->