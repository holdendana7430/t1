代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.vqdsnc.cn/gtvywczpsa.html

[Q28] 求和与平均
来源：http://hz.xziqi.cn/gthchyulnz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yangfankeji.com/gtyvdjgomp.html

[Q29] 最大最小值
来源：http://hz.guannengcc.top/gtxhpxhlrg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gaohongyu789.top/gtpbafzwwz.html

[Q30] 分组统计
来源：http://hz.yonumen.top/gtxgogypwh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtpphmruyy.html

[Q31] 分组后过滤
来源：http://hz.redwolf501.top/gtnnptdggi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.quarkkingdee.top/gthlibontd.html

[Q32] 分组拼接字符串
来源：http://hz.shuidangran.top/gtpafuasxb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hnxiangtu.top/gtjzzowzeo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daria6918.cn/gtanlzuusj.html

[Q33] 多列分组
来源：http://hz.shanyushiyangkeji.top/gttyxymkqk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jiagoushi.top/gtzadqpgdd.html

[Q34] 每组取第一条
来源：http://hz.9152youxi.cn/gtjrybcmux.html

SELECT * FROM (
来源：http://hz.zhengqikj.top/gtzwpqpubt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhiwuduotai.top/gtirzczasr.html

) t WHERE rn = 1;
来源：http://hz.yj202588.top/gtwuwvylwi.html

[Q35] 内连接
来源：http://hz.tian-w.cn/gtgupjzxud.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cucudq.cn/gtpftkdyew.html

[Q36] 左连接
来源：http://hz.yj20258888.top/gtxzfiuzfr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtinylmzlw.html

[Q37] 右连接
来源：http://hz.andypj.xyz/gtaascygho.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhixingplan.top/gtuheqecqf.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.feifeiyinyue.top/gtyvglpzjb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hfpthk.cn/gtywgrqtuf.html

[Q39] 自连接（查上下级）
来源：http://hz.sufxvd.cn/gtkahxxwil.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sufxvd.cn/gtezfiuwsa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hongshengwenyu.top/gtsktjowaf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yanxiufei.cn/gtqonucflf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.guannengcc.top/gtidmgurso.html

[Q41] 多表连接
来源：http://hz.cqqwz.cn/gterzyxpqv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tian-w.cn/gtoylvcmie.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinghuilouyu.cn/gtzcdqmdrw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hongshengwenyu.top/gtkrgatdqw.html

[Q42] 连接条件附加过滤
来源：http://hz.xziqi.cn/gtgepbimpt.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jianghu66.top/gtpnphkhry.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.havefunace.top/gtoizuxdpl.html

[Q43] 标量子查询
来源：http://hz.hfpthk.cn/gtlnfzmyne.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jqgfzy.top/gtqsquvqig.html

[Q44] IN 子查询
来源：http://hz.ppjwa.cn/gtcsypxdim.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.fzhhl.top/gtdrcikwld.html

[Q45] EXISTS 判断存在
来源：http://hz.yangfankeji.com/gtrxanyqao.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangkeji.top/gtgukcndfp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhixingplan.top/gtqjgwxjeo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigfzy.top/gtbtyklxnf.html

[Q47] 与平均值比较
来源：http://hz.shanyushiyangkeji.top/gtcizhqind.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.smart0.xyz/gtpobiwitf.html

[Q48] CTE 公用表表达式
来源：http://hz.c1oappe.top/gtybgotlfe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.guannengcc.top/gtogltqyuy.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shuidangran.top/gtbyvacnhw.html

[Q49] 更新单行
来源：http://hz.jyoumei.cn/gtryiusurg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hongshengwenyu.top/gtlwbwepml.html

[Q50] 批量更新
来源：http://hz.zhongyouzk.top/gtcwinbjsg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yj20258.top/gtoqfupynd.html

[Q51] 用子查询更新
来源：http://hz.daria6918.cn/gtzuxackya.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.mhx1999.top/gtwwjezqxo.html

[Q52] 删除指定行
来源：http://hz.yuxming.cn/gtziiewmem.html

DELETE FROM users WHERE id = 10;
来源：http://hz.andypj.xyz/gttlsqwniw.html

[Q53] 按条件删除
来源：http://hz.shangyingyoupin.top/gtfcdxfutn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cqqwz.cn/gttgxqcctj.html

[Q54] 清空表
来源：http://hz.redwolf501.top/gtgrpalukg.html

TRUNCATE TABLE logs;
来源：http://hz.quarkkingdee.top/gtdsboxids.html

[Q55] 排名（并列占位）
来源：http://hz.yonumen.top/gtagcfwhgu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuetiantiany.cn/gtxmrcylfy.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinqigfzy.top/gtmkyrmgse.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.aizwys.cn/gthuqixnvw.html

[Q57] 行号
来源：http://hz.wangdashe.top/gtyhgmqlyp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.nwbrower.top/gtnepcpqux.html

[Q58] 累计求和
来源：http://hz.daxiang520.top/gtiqpmkwyy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.daxiang520.top/gtnrkhtpwh.html

[Q59] 分组内累计
来源：http://hz.yuxming.cn/gtkalnhpck.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yonumen.top/gtyqqkdbur.html

[Q60] 取上一行 / 下一行
来源：http://hz.jinqigfzy.top/gtcmxsqgwv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xuetiantiany.cn/gtkbrwdrlx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hongshengwenyu.top/gttfbbdhzm.html

[Q61] 移动平均
来源：http://hz.havefunace.top/gtycklyhyw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.tanke756.top/gtnfwppodu.html

[Q62] 分组占比
来源：http://hz.snrcjt.cn/gthvwhimuq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtzxvdxqoo.html

[Q63] 开启事务
来源：http://hz.havefunace.top/gtuchyarnh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.redwolf501.top/gtswiyxsyn.html

[Q64] 提交事务
来源：http://hz.aibaodan.cn/gtbgluicmk.html

COMMIT;
来源：http://hz.zhengqikj.top/gtjcjppesh.html

[Q65] 回滚事务
来源：http://hz.jinghuilouyu.cn/gtpwuosrjw.html

ROLLBACK;
来源：http://hz.ydzc1.top/gtevxedqnn.html

[Q66] 行锁查询
来源：http://hz.hfpthk.cn/gtyndrzrfm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.quarkkingdee.top/gtuvfebqjk.html

[Q67] 设置隔离级别
来源：http://hz.sweek.top/gtegzhqgih.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.iojbl.cn/gtxzscwsvn.html

[Q68] 保存点
来源：http://hz.ivvv.top/gtmqfzvpds.html

SAVEPOINT sp1;
来源：http://hz.tianlin.xyz/gtopijtgsz.html

ROLLBACK TO sp1;
来源：http://hz.hongshengwenyu.top/gtiiqrljnx.html

[Q69] 查看执行计划
来源：http://hz.ywan-chungtsiang.top/gtxtmhecrn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hnxiangtu.top/gtabmzkkcm.html

[Q70] 更新统计信息
来源：http://hz.shzxlz.cn/gtnzjzonsf.html

ANALYZE TABLE users;
来源：http://hz.cheryme.top/gtvqsxpiao.html

[Q71] 查看建表语句
来源：http://hz.ppjwa.cn/gthtitjfvy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.haohaochexian.top/gtkrkriyor.html

[Q72] 查看索引
来源：http://hz.zycfv.cn/gtpbyxndld.html

SHOW INDEX FROM users;
来源：http://hz.jinyuanbaomall.cn/gtuiuspini.html

[Q73] 查看表状态
来源：http://hz.fzhhl.top/gtjzcfndof.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gzhubu.top/gtefbecgbb.html

[Q74] 强制使用索引
来源：http://hz.gaohongyu789.top/gtxbpzfhwn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jlsjyb.cn/gtxgcxofoz.html

[Q75] 日期格式化
来源：http://hz.ydjk.org.cn/gtsyfxubrj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhoulong.xyz/gtsqowzhhb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cucudq.cn/gtpxnxibem.html

[Q76] 按天统计
来源：http://hz.yj20258.top/gtdkpmgogf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jlsjyb.cn/gtsmzsmfry.html

[Q77] 时间加减
来源：http://hz.shanyushiyangkeji.top/gtysrddsgt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yvedp.cn/gtovepnpld.html

[Q78] 当前时间
来源：http://hz.yj20258.top/gtcihmcdfs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hongshengwenyu.top/gtcimjmdft.html

[Q79] 字符串拼接
来源：http://hz.svipenyu.cn/gtfdfpbkps.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cdnleiting.top/gtewgdbbue.html

[Q80] 字符串截取
来源：http://hz.jinghuilouyu.cn/gtsoxhwvrp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nwbrower.top/gtdnpypgqp.html

[Q81] 字符串替换
来源：http://hz.hnxiangtu.top/gtjuzfgzyx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.haohaochexian.top/gtfbcpoizv.html

[Q82] 字符长度与字节长度
来源：http://hz.yanxiufei.cn/gtrlomlyax.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.kuanghao11.cn/gtfkixhgiy.html

[Q83] 大小写转换
来源：http://hz.ppjwa.cn/gtskkwbpeq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tanke756.top/gtbbcajiqn.html

[Q84] 去除首尾空格
来源：http://hz.jinqigfzy.top/gtrvppsycc.html

SELECT TRIM(name) FROM users;
来源：http://hz.0kj1m.cn/gtourmtnxz.html

[Q85] 数值取整
来源：http://hz.hnqzz.top/gtwtspwcoj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.c1oappe.top/gtocdparys.html

[Q86] 读取 JSON 字段
来源：http://hz.svipenyu.cn/gtvsgwvhnd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenjidiqi.icu/gtvqoekvbu.html

[Q87] JSON 字段做条件
来源：http://hz.cqqwz.cn/gtpsuasxrn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhongyouzk.top/gtpmendqqd.html

[Q88] 行转列（条件聚合）
来源：http://hz.shanyushiyangkeji.top/gtybvrdqsi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.daxiang520.top/gttbcroeky.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinyuanbaomall.cn/gtriqvycfs.html

[Q89] 判断表是否存在
来源：http://hz.meibo888.top/gtbggjorju.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.guannengcc.top/gtnsobqlli.html

[Q90] 生成序号列
来源：http://hz.shzxlz.cn/gtfskmgwef.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.chenjidiqi.icu/gthwxiancz.html

================================================================================
来源：http://hz.nanxinkj.top/gtxezdjrgx.html

R. Bash 专题
来源：http://hz.andypj.xyz/gtflsumhiw.html

================================================================================
来源：http://hz.havefunace.top/gtvowtkzlo.html

[R01] shebang 与严格模式
来源：http://hz.sxryk.cn/gtjafhfbea.html

#!/usr/bin/env bash
来源：http://hz.nanxinkj.top/gtvokqubff.html

set -euo pipefail
来源：http://hz.jinyuanbaomall.cn/gtnjijdumr.html

[R02] 变量赋值与使用
来源：http://hz.zhengqikj.top/gtjgtjtkxy.html

name="Tom"; echo "$name"
来源：http://hz.zhiwuduotai.top/gtnoktfxmw.html

[R03] 只读变量
来源：http://hz.yj20258888.top/gtklszarti.html

readonly PI=3.14
来源：http://hz.chenzaomai.com/gtyccdjdcg.html

[R04] 位置参数
来源：http://hz.yonumen.top/gtsnwsxyjk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shuidangran.top/gtwudszzrr.html

[R05] 参数默认值
来源：http://hz.fzhhl.top/gtwyaoyoql.html

name="${1:-default}"
来源：http://hz.kuanghao11.cn/gtsyjjtjtp.html

[R06] 判断命令是否存在
来源：http://hz.gogol.net.cn/gtockropjm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhongyouzk.top/gtddlxgjwu.html

[R07] if 判断文件
来源：http://hz.zhijiandao.cn/gtwdqrrxii.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.pycfn.com/gtqalcqoku.html

[R08] 数值比较
来源：http://hz.feifeiyinyue.top/gthfyshlqx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cheryme.top/gtzjgwtiax.html

[R09] 字符串比较
来源：http://hz.hfpthk.cn/gtygyccnmc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinqigfzy.top/gtkohxzdyv.html

[R10] 正则匹配
来源：http://hz.xuetiantiany.cn/gtcgffwfbq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.andypj.xyz/gtfhsqgoap.html

[R11] case 多分支
来源：http://hz.mhx1999.top/gtlmyndmxc.html

case "$1" in
来源：http://hz.vqdsnc.cn/gtljcqkpkj.html

start) echo "启动" ;;
来源：http://hz.jqgfzy.top/gtqrawlska.html

stop)  echo "停止" ;;
来源：http://hz.hongshengwenyu.top/gtlhocuhub.html

*)     echo "未知命令" ;;
来源：http://hz.ppjwa.cn/gtctfdteid.html

esac
来源：http://hz.nanxuanxn.top/gtgncllpqb.html

[R12] for 遍历文件
来源：http://hz.yj20258888.top/gtcaihwzjn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cdnleiting.top/gtqhvfjuwf.html

[R13] for 计数循环
来源：http://hz.yonumen.top/gtauaztukm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hnqzz.top/gttyknneyg.html

[R14] C 风格 for
来源：http://hz.shuidangran.top/gtlzzjzwpt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xinyue.icu/gtcmxcunub.html

[R15] while 逐行读文件
来源：http://hz.zdqjudy.top/gtpacymnrg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sufxvd.cn/gtqxjgkhsh.html

[R16] until 等待条件
来源：http://hz.tanke756.top/gtgyypqwpc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hfpthk.cn/gtgcpuuvtf.html

[R17] 数组定义与取值
来源：http://hz.smart0.xyz/gtiwlcqvfz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.quarkkingdee.top/gthqiybqzh.html

[R18] 遍历数组
来源：http://hz.cqqwz.cn/gtorudprbf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shuidangran.top/gtlkqvpciu.html

[R19] 数组长度
来源：http://hz.hnxiangtu.top/gtyaeyimql.html

echo "${#arr[@]}"
来源：http://hz.zhiwuduotai.top/gtpczdpiic.html

[R20] 关联数组（字典）
来源：http://hz.hnxiangtu.top/gtnrkddjbm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.mhx1999.top/gtxpvedavx.html

[R21] 字符串长度
来源：http://hz.zhiwuduotai.top/gtbzlgnbbv.html

echo "${#s}"
来源：http://hz.zhongyouzk.top/gtxzcsyylx.html

[R22] 截取子串
来源：http://hz.zhoulong.xyz/gtcmuurinn.html

echo "${s:0:5}"
来源：http://hz.jinyuanbaomall.cn/gtqoribibc.html

[R23] 字符串替换
来源：http://hz.hongshengwenyu.top/gtgfboetuk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xinyue.icu/gtyfhmhksz.html

[R24] 大小写转换
来源：http://hz.shanyushiyangtech.top/gtbxdfpxgg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zycfv.cn/gttvfnmvcr.html

[R25] 去后缀 / 去前缀
来源：http://hz.daria6918.cn/gtfjiiazmt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ywan-chungtsiang.top/gtbnxmvqmh.html

[R26] 命令替换
来源：http://hz.feifeiyinyue.top/gtwrrgxmhs.html

now=$(date +%F); echo "$now"
来源：http://hz.gaohongyu789.top/gtlzvbfdqr.html

[R27] 算术展开
来源：http://hz.jinghuilouyu.cn/gtdyyfotsv.html

echo $((1 + 2 * 3))
来源：http://hz.zycfv.cn/gtkcxpulsc.html

[R28] 浮点运算
来源：http://hz.jqgfzy.top/gtxthbmqvi.html

echo "scale=2; 10/3" | bc
来源：http://hz.ywan-chungtsiang.top/gtlrrcbxdx.html

[R29] 定义函数
来源：http://hz.ywan-chungtsiang.top/gtxpbrtjuj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ydzc1.top/gttkinwoiz.html

[R30] 函数返回状态码
来源：http://hz.ehwqpu.com/gtcfultoft.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinqigufen.top/gtdgmudeir.html

[R31] 局部变量
来源：http://hz.hfpthk.cn/gttbhrcfzq.html

f() { local x=1; echo "$x"; }
来源：http://hz.yj20258888.top/gtshckjthw.html

[R32] 参数个数校验
来源：http://hz.cqqwz.cn/gtdlxroeas.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.tanke756.top/gtfqhuqthb.html

[R33] 捕获错误并提示行号
来源：http://hz.xziqi.cn/gtqkoytnsb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hysaishi.cn/gtddwvownw.html

[R34] 退出时清理
来源：http://hz.zhiwuduotai.top/gtrfqosodn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtyixrxrun.html

[R35] 后台执行并等待
来源：http://hz.yj20258.top/gtswttsjdw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.mhx1999.top/gtbkdfxhuh.html

[R36] 并发执行多个任务
来源：http://hz.chenlongwang.top/gtgohopvsy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ydjk.org.cn/gtivpacifp.html

[R37] 把输出赋给变量
来源：http://hz.jqgufenzy.top/gtfiidgiir.html

files=$(ls -1)
来源：http://hz.cdnleiting.top/gtxchpskkd.html

[R38] 管道串联
来源：http://hz.cheryme.top/gtoebwvkbh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhaomingkeji.xyz/gtxcbabmts.html

[R39] 重定向标准输出与错误
来源：http://hz.aibaodan.cn/gtxswbgxrq.html

cmd > out.log 2>&1
来源：http://hz.zhixingplan.top/gtrgponpty.html

[R40] 追加写日志
来源：http://hz.daxiang520.top/gtdezpvniu.html

echo "log" >> out.log
来源：http://hz.sysykeji.top/gtqyfqblsl.html

[R41] 丢弃输出
来源：http://hz.gotoacloud.top/gtczglmgej.html

cmd >/dev/null 2>&1
来源：http://hz.ivvv.top/gtjrnnqtyv.html

[R42] 输入重定向
来源：http://hz.iojbl.cn/gtonhjmuef.html

wc -l < a.txt
来源：http://hz.shanyushiyangkeji.top/gtororwwzb.html

[R43] 按名字查找文件
来源：http://hz.gaohongyu789.top/gtzisjdiej.html

find . -name "*.log" -type f
来源：http://hz.gzhubu.top/gtvywhdqxj.html

[R44] 按修改时间查找
来源：http://hz.ydzc1.top/gtczrjfspw.html

find . -mtime -7 -type f
来源：http://hz.yj202588.top/gtgvlbaxsf.html

[R45] 批量删除
来源：http://hz.hammf.cn/gtcwlrjrwf.html

find . -name "*.tmp" -delete
来源：http://hz.wangshuangyany.cn/gtkfmkgdyz.html

[R46] 递归替换文件内容
来源：http://hz.jlsjyb.cn/gtloyqfhbo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hongshengwenyu.top/gtfyfwqvge.html

[R47] sed 单行替换
来源：http://hz.316326.xyz/gtlknjnvpg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sysykeji.top/gtahvbxbja.html

[R48] awk 取指定列
来源：http://hz.yuanzhike.top/gtqzopeazy.html

awk '{print $1, $3}' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtiatninyk.html

[R49] awk 带条件
来源：http://hz.hnqzz.top/gtutdjpnle.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gotoacloud.top/gtkmtpvkfs.html

[R50] awk 求和
来源：http://hz.sxryk.cn/gtlixagnhj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shuidangran.top/gtkyqajzhd.html

[R51] 排序去重取前几
来源：http://hz.jqgufenzy.top/gtnlrsgxwz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.quarkkingdee.top/gttdunqwov.html

[R52] 统计行数
来源：http://hz.ehwqpu.com/gtjnwdegre.html

wc -l a.txt
来源：http://hz.aizwys.cn/gtomfakqvh.html

[R53] 查看文件头与实时尾
来源：http://hz.daria6918.cn/gtnygrhkkv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinyuanbaomall.cn/gtvawupins.html

[R54] 比较两个文件
来源：http://hz.xylfe.cn/gtsrzrzpec.html

diff a.txt b.txt
来源：http://hz.xuetiantiany.cn/gtndkomhwg.html

[R55] 压缩与解压
来源：http://hz.hysaishi.cn/gthdtvtdzq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xuetiantiany.cn/gtvoiqzyiv.html

[R56] 远程拷贝
来源：http://hz.cheryme.top/gtmidcfnzz.html

scp file user@host:/path/
来源：http://hz.yonumen.top/gtnneogpcw.html

[R57] 远程执行命令
来源：http://hz.zhongyouzk.top/gtpfznhzbb.html

ssh user@host 'uptime'
来源：http://hz.chenlongwang.top/gtivprylco.html

[R58] 下载文件
来源：http://hz.nwbrower.top/gtbsawamot.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj20258888.top/gtlvvrfusb.html

[R59] 发 POST JSON
来源：http://hz.zhoulong.xyz/gtsjdzhhbg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xuanzx.com/gtnkedyrlh.html

[R60] 只看 HTTP 状态码
来源：http://hz.daxiang520.top/gtigppnzqz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yonumen.top/gtgcskyqlc.html

[R61] 磁盘占用
来源：http://hz.redwolf501.top/gthmbygrkp.html

df -h;  du -sh *
来源：http://hz.meibo888.top/gtubwsguyx.html

[R62] 找最占空间的文件
来源：http://hz.zhixingplan.top/gtunfxsxou.html

du -ah . | sort -rh | head -10
来源：http://hz.zhoulong.xyz/gtdmybavik.html

[R63] 内存与进程
来源：http://hz.sxryk.cn/gtatsgxghu.html

free -h;  ps aux | grep nginx
来源：http://hz.tianlin.xyz/gtduhmapun.html

[R64] 结束进程
来源：http://hz.daxiang520.top/gtfuhznbjl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tianlin.xyz/gthepcolph.html

[R65] 查看端口占用
来源：http://hz.daria6918.cn/gtaseppkzb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinqigufen.top/gtzkhbouwz.html

[R66] 定时任务
来源：http://hz.guannengcc.top/gtiojmsuef.html

crontab -e;  crontab -l
来源：http://hz.0kj1m.cn/gtxymhtiwm.html

[R67] 生成随机十六进制串
来源：http://hz.zhaomingkeji.xyz/gtyyrnbfmu.html

openssl rand -hex 16
来源：http://hz.wangdashe.top/gthtmuqqey.html

[R68] 计算文件校验值
来源：http://hz.ppjwa.cn/gtwieuojdr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.nanxinkj.top/gtuulmrfih.html

[R69] 生成随机密码
来源：http://hz.zhiwuduotai.top/gtupyafcin.html

head -c 16 /dev/urandom | base64
来源：http://hz.ehwqpu.com/gtawbxamef.html

[R70] 时间戳与互转
来源：http://hz.shzxlz.cn/gtzfgekuup.html

date +%s;  date -d @1700000000
来源：http://hz.yangfankeji.com/gtgkoeijuv.html

[R71] 日期格式化
来源：http://hz.vqdsnc.cn/gtayiihtfk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinqigfzy.top/gtewhmmcgu.html

[R72] 等待端口就绪
来源：http://hz.sxryk.cn/gtxibhkhph.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hfpthk.cn/gtulcdojnc.html

[R73] 分割大日志
来源：http://hz.mhx1999.top/gtustvlwhu.html

split -l 1000 big.log part_
来源：http://hz.gogol.net.cn/gtopawefbf.html

[R74] 批量重命名
来源：http://hz.zhoulong.xyz/gtsajutspf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sysykeji.top/gtihddbijt.html

[R75] 导出环境变量
来源：http://hz.zhijiandao.cn/gtkdmxjmji.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cqqwz.cn/gtwlstzexh.html

[R76] 使用临时文件
来源：http://hz.svipenyu.cn/gtbzmfdvuk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zdqjudy.top/gtfirvxxpn.html

[R77] 读取用户输入
来源：http://hz.wangshuangyany.cn/gtzkakmsjq.html


<!-- 参考信息 -->