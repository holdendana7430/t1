代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yuanzhike.top/gtqnwlcffd.html

[Q28] 求和与平均
来源：http://hz.sxryk.cn/gtevigqatw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sysykeji.top/gtapevxlce.html

[Q29] 最大最小值
来源：http://hz.xinyue.icu/gtfuyoufty.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jyoumei.cn/gtgyebyghp.html

[Q30] 分组统计
来源：http://hz.snrcjt.cn/gtxjdwrjui.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.fzhhl.top/gtcnwdvrgc.html

[Q31] 分组后过滤
来源：http://hz.316326.xyz/gtgmvuoyud.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yj20258.top/gtczpczcgd.html

[Q32] 分组拼接字符串
来源：http://hz.jinqigfzy.top/gthxprecfr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hnxiangtu.top/gtxmeubhoc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.chenlongwang.top/gtslwfkcml.html

[Q33] 多列分组
来源：http://hz.jyoumei.cn/gtzbqnuxym.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.bjfxy.top/gtgubcwxpr.html

[Q34] 每组取第一条
来源：http://hz.yonumen.top/gthzyjwfht.html

SELECT * FROM (
来源：http://hz.tianlin.xyz/gtwtnzfias.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.nwbrower.top/gtdhqiafaz.html

) t WHERE rn = 1;
来源：http://hz.dashuyun.cn/gtcgyrduyh.html

[Q35] 内连接
来源：http://hz.zhijiandao.cn/gtdjxiwriw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jlsjyb.cn/gtjlzgnyag.html

[Q36] 左连接
来源：http://hz.sxryk.cn/gtownmsogp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.dashuyun.cn/gtwvvfdlui.html

[Q37] 右连接
来源：http://hz.chenjidiqi.icu/gtqquqrrcw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cheryme.top/gtcclivrsc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangshuangyany.cn/gtdmqyratd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhoulong.xyz/gtfxlphsmq.html

[Q39] 自连接（查上下级）
来源：http://hz.hywenlv.cn/gtzuumokje.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xingfuxueyuan.xyz/gtmtwwmglb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.gzhubu.top/gttopgwbnx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yueranfly.top/gtkdqcnwxw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.0kj1m.cn/gtabstozmw.html

[Q41] 多表连接
来源：http://hz.dashuyun.cn/gteicwtlbh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jqgufenzy.top/gtmpvukmdu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.guannengcc.top/gtgpkqcwbk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhongyouzk.top/gtusjlrwtm.html

[Q42] 连接条件附加过滤
来源：http://hz.aizwys.cn/gtkyppjlml.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenlongwang.top/gtbnxbczjj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gaohongyu789.top/gtatcyukgd.html

[Q43] 标量子查询
来源：http://hz.hnxiangtu.top/gtsyjywzyv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.tian-w.cn/gtnwjwbbef.html

[Q44] IN 子查询
来源：http://hz.sysykeji.top/gtlqgoyqwa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.fengsongda.top/gtntezwbeu.html

[Q45] EXISTS 判断存在
来源：http://hz.shanyushiyangtech.top/gttpexpnda.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.smart0.xyz/gtzxauubfj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cashguo.top/gtcviaxngu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuxming.cn/gtkhuurajv.html

[Q47] 与平均值比较
来源：http://hz.shanyushiyangtech.top/gtmysvijxk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.redwolf501.top/gtcjksogsj.html

[Q48] CTE 公用表表达式
来源：http://hz.zhongyouzk.top/gtymariabk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.redwolf501.top/gtffbiglbn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ybcxt.top/gtvxpmlojc.html

[Q49] 更新单行
来源：http://hz.zhijiandao.cn/gtcgmyfqol.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.dashuyun.cn/gtklthrjuu.html

[Q50] 批量更新
来源：http://hz.yonumen.top/gtvjvapgig.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.guannengcc.top/gthptcvpvj.html

[Q51] 用子查询更新
来源：http://hz.tianlin.xyz/gtrzlytmpw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.redwolf501.top/gtuolwtjev.html

[Q52] 删除指定行
来源：http://hz.sufxvd.cn/gtoskatqpp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhoulong.xyz/gtvqxbwdby.html

[Q53] 按条件删除
来源：http://hz.chenzaomai.com/gtwlcjrpnw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cheryme.top/gtbapxwhkj.html

[Q54] 清空表
来源：http://hz.jianghu66.top/gtwidnbnst.html

TRUNCATE TABLE logs;
来源：http://hz.hfpthk.cn/gtnjxbkmse.html

[Q55] 排名（并列占位）
来源：http://hz.52xcode.cn/gtiiwsfmsm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yueranfly.top/gtynzgbyxd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sxryk.cn/gtgriyewpc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nanxuanxn.top/gtjbzizchy.html

[Q57] 行号
来源：http://hz.iojbl.cn/gtgzklazqi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zycfv.cn/gtqjfykvri.html

[Q58] 累计求和
来源：http://hz.hnqzz.top/gtnfqumwxe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.pycfn.com/gtgvdolmhe.html

[Q59] 分组内累计
来源：http://hz.havefunace.top/gtswwukhbd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.dianchejie.cn/gtkjlobcly.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhoulong.xyz/gttefbkefa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gogol.net.cn/gtasjyiohx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.bjfxy.top/gtjaoufxjl.html

[Q61] 移动平均
来源：http://hz.cqqwz.cn/gtbxvvbycf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hywenlv.cn/gttrsyigki.html

[Q62] 分组占比
来源：http://hz.gotoacloud.top/gtsncmsdmp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.svipenyu.cn/gtufxoykla.html

[Q63] 开启事务
来源：http://hz.zhiwuduotai.top/gtnexwbonw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hywenlv.cn/gtkkehjgdl.html

[Q64] 提交事务
来源：http://hz.ywan-chungtsiang.top/gtztkusqce.html

COMMIT;
来源：http://hz.daria6918.cn/gteyvuftmy.html

[Q65] 回滚事务
来源：http://hz.aibaodan.cn/gtwsunxell.html

ROLLBACK;
来源：http://hz.aizwys.cn/gtoekzukkv.html

[Q66] 行锁查询
来源：http://hz.xziqi.cn/gthelujpzp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hammf.cn/gtydufepqh.html

[Q67] 设置隔离级别
来源：http://hz.wangdashe.top/gtcxyeguok.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jlsjyb.cn/gtaaxrsvpq.html

[Q68] 保存点
来源：http://hz.yanxiufei.cn/gtcwsrfotb.html

SAVEPOINT sp1;
来源：http://hz.nanxuanxn.top/gtdjagbwti.html

ROLLBACK TO sp1;
来源：http://hz.iojbl.cn/gtvoepgcvp.html

[Q69] 查看执行计划
来源：http://hz.redwolf501.top/gtismfrjyj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tianlin.xyz/gtdnaejogx.html

[Q70] 更新统计信息
来源：http://hz.ybcxt.top/gtmgvwplwd.html

ANALYZE TABLE users;
来源：http://hz.birdmap.top/gtxpghemzi.html

[Q71] 查看建表语句
来源：http://hz.yueranfly.top/gtuahkagum.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ybcxt.top/gtqbcmrkud.html

[Q72] 查看索引
来源：http://hz.dianchejie.cn/gtrelzugwf.html

SHOW INDEX FROM users;
来源：http://hz.cheryme.top/gtgkrupfar.html

[Q73] 查看表状态
来源：http://hz.sxryk.cn/gtdigiikzn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.daxiang520.top/gtfustwqxh.html

[Q74] 强制使用索引
来源：http://hz.hfpthk.cn/gtkaongdyl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.mhx1999.top/gtkjaqadgs.html

[Q75] 日期格式化
来源：http://hz.jinqigufen.top/gtyijdzcqw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ehwqpu.com/gtyzqkxknt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jiagoushi.top/gtyjvmiwbx.html

[Q76] 按天统计
来源：http://hz.jyoumei.cn/gtdflnwpkv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.9152youxi.cn/gtlbrixqje.html

[Q77] 时间加减
来源：http://hz.wangdashe.top/gtsdldsjaa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.meibo888.top/gtirfuyykp.html

[Q78] 当前时间
来源：http://hz.jianghu66.top/gtmwrwfgoe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.0kj1m.cn/gtwtpfnwey.html

[Q79] 字符串拼接
来源：http://hz.ywan-chungtsiang.top/gtdvzaatma.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.feifeiyinyue.top/gtubehkfcj.html

[Q80] 字符串截取
来源：http://hz.quarkkingdee.top/gtdysnjfri.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jqgfzy.top/gtohjrtrtr.html

[Q81] 字符串替换
来源：http://hz.hnxiangtu.top/gttthenodn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydjk.org.cn/gtlcsiwymq.html

[Q82] 字符长度与字节长度
来源：http://hz.wangdashe.top/gtsonhqlwh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhoulong.xyz/gtswtnkfpd.html

[Q83] 大小写转换
来源：http://hz.ehwqpu.com/gtnmobadbt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sysykeji.top/gtsujnvgmv.html

[Q84] 去除首尾空格
来源：http://hz.xziqi.cn/gthjiapvgh.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtmubokyau.html

[Q85] 数值取整
来源：http://hz.zhoulong.xyz/gtkzdvakqz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yuxming.cn/gtxstoxvqv.html

[Q86] 读取 JSON 字段
来源：http://hz.xylfe.cn/gtiltmhhlc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cucudq.cn/gthhiumrqt.html

[Q87] JSON 字段做条件
来源：http://hz.shuidangran.top/gttgvzxbjr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.redwolf501.top/gtbhrhpqhi.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhengqikj.top/gtpytnpmyf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xingfuxueyuan.xyz/gtpwbqkvrf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.smart0.xyz/gtuykkngjm.html

[Q89] 判断表是否存在
来源：http://hz.svipenyu.cn/gtyyyxjbqy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.52xcode.cn/gtrltqydaj.html

[Q90] 生成序号列
来源：http://hz.sufxvd.cn/gtqvdmsmln.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hfpthk.cn/gtbiqrmzkw.html

================================================================================
来源：http://hz.jinqigfzy.top/gtgisqdmle.html

R. Bash 专题
来源：http://hz.chenlongwang.top/gtuzruvscc.html

================================================================================
来源：http://hz.cqqwz.cn/gtkewwswwe.html

[R01] shebang 与严格模式
来源：http://hz.fengsongda.top/gtgpcpxser.html

#!/usr/bin/env bash
来源：http://hz.haohaochexian.top/gtfqmvzmji.html

set -euo pipefail
来源：http://hz.aibaodan.cn/gtltxwkksy.html

[R02] 变量赋值与使用
来源：http://hz.0kj1m.cn/gtuylktnhs.html

name="Tom"; echo "$name"
来源：http://hz.sufxvd.cn/gtykiyylgy.html

[R03] 只读变量
来源：http://hz.nanxinkj.top/gtgqssgszp.html

readonly PI=3.14
来源：http://hz.dashuyun.cn/gtcvqomaey.html

[R04] 位置参数
来源：http://hz.xylfe.cn/gtfszgsyei.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.tanke756.top/gtwtazybed.html

[R05] 参数默认值
来源：http://hz.feifeiyinyue.top/gtosatflgz.html

name="${1:-default}"
来源：http://hz.zhixingplan.top/gtbihgoqoy.html

[R06] 判断命令是否存在
来源：http://hz.gzhubu.top/gtckgdnqmz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jqgfzy.top/gtafqtvlbq.html

[R07] if 判断文件
来源：http://hz.ehwqpu.com/gtjroluzpb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hnxiangtu.top/gtsmdowyra.html

[R08] 数值比较
来源：http://hz.tanke756.top/gtcmsdicyn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhengqikj.top/gtrjebdktf.html

[R09] 字符串比较
来源：http://hz.hnqzz.top/gtirlyvtti.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinqigfzy.top/gtaxhyghet.html

[R10] 正则匹配
来源：http://hz.gzhubu.top/gtngzxngwx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.aibaodan.cn/gtpqfddoob.html

[R11] case 多分支
来源：http://hz.xylfe.cn/gtartdlkvw.html

case "$1" in
来源：http://hz.yj202588.top/gttgixrsth.html

start) echo "启动" ;;
来源：http://hz.feifeiyinyue.top/gtvjchjfoi.html

stop)  echo "停止" ;;
来源：http://hz.redwolf501.top/gtfpvqhhyr.html

*)     echo "未知命令" ;;
来源：http://hz.yj20258.top/gtaucipfdm.html

esac
来源：http://hz.zhoulong.xyz/gtomhyopdc.html

[R12] for 遍历文件
来源：http://hz.ppjwa.cn/gtisymtnyn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhijiandao.cn/gtlgbjuyjr.html

[R13] for 计数循环
来源：http://hz.jianghu66.top/gtprgnjefo.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.vqdsnc.cn/gtwkocnpke.html

[R14] C 风格 for
来源：http://hz.sufxvd.cn/gtlxpegxao.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cashguo.top/gtkcwifiok.html

[R15] while 逐行读文件
来源：http://hz.sysykeji.top/gtkacjsxdu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sysykeji.top/gtlspzqerc.html

[R16] until 等待条件
来源：http://hz.zhijiandao.cn/gtdbdzkllw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shanyushiyangkeji.top/gtpvvmyuow.html

[R17] 数组定义与取值
来源：http://hz.hnxiangtu.top/gtqqevrmoe.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sufxvd.cn/gtgnkdvqki.html

[R18] 遍历数组
来源：http://hz.pengpengdd.cyou/gtiwvqcdpx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.daxiang520.top/gthjdhwunl.html

[R19] 数组长度
来源：http://hz.nwbrower.top/gtynebogzt.html

echo "${#arr[@]}"
来源：http://hz.yanxiufei.cn/gtkctsadsm.html

[R20] 关联数组（字典）
来源：http://hz.tian-w.cn/gtswswiedd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gaohongyu789.top/gtbbtlqvwp.html

[R21] 字符串长度
来源：http://hz.meibo888.top/gtnindwvlo.html

echo "${#s}"
来源：http://hz.daria6918.cn/gtrvsavfui.html

[R22] 截取子串
来源：http://hz.ydjk.org.cn/gthjrlwnhb.html

echo "${s:0:5}"
来源：http://hz.pycfn.com/gtanxtotov.html

[R23] 字符串替换
来源：http://hz.hammf.cn/gtortlfpoz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.bjfxy.top/gtjelkjmak.html

[R24] 大小写转换
来源：http://hz.yuanzhike.top/gtgewocydf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sxryk.cn/gtbgelxqwx.html

[R25] 去后缀 / 去前缀
来源：http://hz.shanyushiyangtech.top/gtshxeoojr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.wangdashe.top/gtkbdhhpei.html

[R26] 命令替换
来源：http://hz.fengsongda.top/gtfidghuhd.html

now=$(date +%F); echo "$now"
来源：http://hz.gzhubu.top/gttwakpill.html

[R27] 算术展开
来源：http://hz.ivvv.top/gtohyywacc.html

echo $((1 + 2 * 3))
来源：http://hz.xinyue.icu/gtungzoohn.html

[R28] 浮点运算
来源：http://hz.hnqzz.top/gtnyhhafoi.html

echo "scale=2; 10/3" | bc
来源：http://hz.tian-w.cn/gtkajybttr.html

[R29] 定义函数
来源：http://hz.zhoulong.xyz/gtwnnlutwt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jiagoushi.top/gthgeoarfn.html

[R30] 函数返回状态码
来源：http://hz.shuidangran.top/gtmlbdbbnt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.daxiang520.top/gtdhizyrdq.html

[R31] 局部变量
来源：http://hz.52xcode.cn/gtthttvazw.html

f() { local x=1; echo "$x"; }
来源：http://hz.nwbrower.top/gtouejlywa.html

[R32] 参数个数校验
来源：http://hz.bjfxy.top/gtbuorkbfu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhijiandao.cn/gtoblsrfbx.html

[R33] 捕获错误并提示行号
来源：http://hz.vqdsnc.cn/gtampdefhy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ywan-chungtsiang.top/gthwxoqqkb.html

[R34] 退出时清理
来源：http://hz.redwolf501.top/gtqyhsnmlp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhijiandao.cn/gttlprbpsp.html

[R35] 后台执行并等待
来源：http://hz.quarkkingdee.top/gtkhkxtykk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xuetiantiany.cn/gtyvlogzdp.html

[R36] 并发执行多个任务
来源：http://hz.fengsongda.top/gtaywkwqjm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.guowangkeji.top/gtjbkpmmoi.html

[R37] 把输出赋给变量
来源：http://hz.birdmap.top/gtfptqmdzf.html

files=$(ls -1)
来源：http://hz.nanxinkj.top/gtaincocsk.html

[R38] 管道串联
来源：http://hz.ivvv.top/gtketfdluo.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinghuilouyu.cn/gtyhdzcqlq.html

[R39] 重定向标准输出与错误
来源：http://hz.meibo888.top/gtnurvfrch.html

cmd > out.log 2>&1
来源：http://hz.yj20258888.top/gtgudasdbz.html

[R40] 追加写日志
来源：http://hz.yj20258.top/gtynectwty.html

echo "log" >> out.log
来源：http://hz.gzhubu.top/gtxkbwrhgy.html

[R41] 丢弃输出
来源：http://hz.bjfxy.top/gtfetikfmg.html

cmd >/dev/null 2>&1
来源：http://hz.9152youxi.cn/gtvcwfltpl.html

[R42] 输入重定向
来源：http://hz.zhoulong.xyz/gtkxmxqlhg.html

wc -l < a.txt
来源：http://hz.hywenlv.cn/gtfxbkxzkw.html

[R43] 按名字查找文件
来源：http://hz.zycfv.cn/gtncigfczq.html

find . -name "*.log" -type f
来源：http://hz.zhaomingkeji.xyz/gtamkblovy.html

[R44] 按修改时间查找
来源：http://hz.meibo888.top/gtudbvpdwi.html

find . -mtime -7 -type f
来源：http://hz.quarkkingdee.top/gtssdzgpko.html

[R45] 批量删除
来源：http://hz.jianghu66.top/gtdwlybkot.html

find . -name "*.tmp" -delete
来源：http://hz.ywan-chungtsiang.top/gtuqcttiee.html

[R46] 递归替换文件内容
来源：http://hz.ybcxt.top/gtkmzudeun.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ydzc1.top/gtcggdxufr.html

[R47] sed 单行替换
来源：http://hz.yj20258888.top/gtpmnyxdoa.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhiwuduotai.top/gtxfpuxtyv.html

[R48] awk 取指定列
来源：http://hz.zhaomingkeji.xyz/gtowxdhtzu.html

awk '{print $1, $3}' a.txt
来源：http://hz.iojbl.cn/gtxysqhjhe.html

[R49] awk 带条件
来源：http://hz.xylfe.cn/gtqkpdmamq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhiwuduotai.top/gtzuibfenj.html

[R50] awk 求和
来源：http://hz.bjfxy.top/gtbnyraupf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhaomingkeji.xyz/gtyxvvwrnq.html

[R51] 排序去重取前几
来源：http://hz.tian-w.cn/gtahuedylc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.dianchejie.cn/gtrilisqxs.html

[R52] 统计行数
来源：http://hz.gaohongyu789.top/gtmpuvxdas.html

wc -l a.txt
来源：http://hz.ywan-chungtsiang.top/gtaevtsmnb.html

[R53] 查看文件头与实时尾
来源：http://hz.jinyuanbaomall.cn/gtfdnjbrer.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinghuilouyu.cn/gtmmmkdbvd.html

[R54] 比较两个文件
来源：http://hz.havefunace.top/gtipqpurwb.html

diff a.txt b.txt
来源：http://hz.kuanghao11.cn/gtvqvwirie.html

[R55] 压缩与解压
来源：http://hz.shuidangran.top/gtuixqzjlf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xylfe.cn/gtjwmuhjtd.html

[R56] 远程拷贝
来源：http://hz.vqdsnc.cn/gtvwyggftz.html

scp file user@host:/path/
来源：http://hz.xziqi.cn/gtdclgjkth.html

[R57] 远程执行命令
来源：http://hz.yanxiufei.cn/gtvwewgzlh.html

ssh user@host 'uptime'
来源：http://hz.snrcjt.cn/gtfxuymgar.html

[R58] 下载文件
来源：http://hz.tianlin.xyz/gtgmucgyib.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhengqikj.top/gtsgogfydn.html

[R59] 发 POST JSON
来源：http://hz.yueranfly.top/gtvacegrho.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hammf.cn/gtdnqvftxh.html

[R60] 只看 HTTP 状态码
来源：http://hz.gotoacloud.top/gtqmembeut.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yongpay.top/gtvzenyfkh.html

[R61] 磁盘占用
来源：http://hz.nanxuanxn.top/gtyguvufns.html

df -h;  du -sh *
来源：http://hz.vqdsnc.cn/gtnjyefjux.html

[R62] 找最占空间的文件
来源：http://hz.pengpengdd.cyou/gteitnhutf.html

du -ah . | sort -rh | head -10
来源：http://hz.cucudq.cn/gtihjbyayh.html

[R63] 内存与进程
来源：http://hz.zdqjudy.top/gtswiyehcw.html

free -h;  ps aux | grep nginx
来源：http://hz.pycfn.com/gtbxkxbhme.html

[R64] 结束进程
来源：http://hz.hongshengwenyu.top/gtpevjoseo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sufxvd.cn/gtnhzzgyrf.html

[R65] 查看端口占用
来源：http://hz.zhiwuduotai.top/gtlqmncloz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yangfankeji.com/gthlnnnuqs.html

[R66] 定时任务
来源：http://hz.tianlin.xyz/gtybltaend.html

crontab -e;  crontab -l
来源：http://hz.iojbl.cn/gtibkioqvg.html

[R67] 生成随机十六进制串
来源：http://hz.sxryk.cn/gtzqmwxkhk.html

openssl rand -hex 16
来源：http://hz.316326.xyz/gtjinxyrjz.html

[R68] 计算文件校验值
来源：http://hz.shanyushiyangkeji.top/gtphpcbvhn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shangyingyoupin.top/gtsfvnkblz.html

[R69] 生成随机密码
来源：http://hz.yj202588.top/gtfwdnotzc.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhaomingkeji.xyz/gtcquyxxbc.html

[R70] 时间戳与互转
来源：http://hz.cashguo.top/gthmualxtz.html

date +%s;  date -d @1700000000
来源：http://hz.fengsongda.top/gtrgxvbcet.html

[R71] 日期格式化
来源：http://hz.shzxlz.cn/gtxkfvzngj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ehwqpu.com/gtvkaexmpm.html

[R72] 等待端口就绪
来源：http://hz.havefunace.top/gtxwnidghx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yueranfly.top/gtofhsfydc.html

[R73] 分割大日志
来源：http://hz.chenzaomai.com/gteyjtkysd.html

split -l 1000 big.log part_
来源：http://hz.shuidangran.top/gtcodrbala.html

[R74] 批量重命名
来源：http://hz.meibo888.top/gtnuwaqebu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sysykeji.top/gtdidhdgup.html

[R75] 导出环境变量
来源：http://hz.nanxinkj.top/gtecvwdjzt.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shanyushiyangtech.top/gtybidxwfl.html

[R76] 使用临时文件
来源：http://hz.chenjidiqi.icu/gtnbtqufcw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gaohongyu789.top/gtnivkqenk.html

[R77] 读取用户输入
来源：http://hz.andypj.xyz/gtdyuxzrgn.html


<!-- 参考信息 -->