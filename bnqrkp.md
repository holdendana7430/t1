代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.wangshuangyany.cn/gthaezjmdj.html

[Q26] 计数
来源：http://hz.yj202588.top/gtcuwebcsv.html

SELECT COUNT(*) FROM users;
来源：http://hz.316326.xyz/gtocccweud.html

[Q27] 条件计数
来源：http://hz.c1oappe.top/gtacrpqfas.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.havefunace.top/gtxltdtgfk.html

[Q28] 求和与平均
来源：http://hz.yj20258888.top/gtzhprivqt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.wangdashe.top/gtqwgdnpmz.html

[Q29] 最大最小值
来源：http://hz.shzxlz.cn/gtfiqvuvpr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yonumen.top/gttnqhorva.html

[Q30] 分组统计
来源：http://hz.vqdsnc.cn/gtlqnmxhat.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtdhqjnnfx.html

[Q31] 分组后过滤
来源：http://hz.dashuyun.cn/gtrgfpdedn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.52xcode.cn/gtmxdfilgs.html

[Q32] 分组拼接字符串
来源：http://hz.c1oappe.top/gtuubsguqa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zdqjudy.top/gtacmlyprb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.guowangkeji.top/gtwgovxtax.html

[Q33] 多列分组
来源：http://hz.jqgufenzy.top/gtkmnzbztp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sysykeji.top/gturfjqtpx.html

[Q34] 每组取第一条
来源：http://hz.316326.xyz/gtevhjfvpo.html

SELECT * FROM (
来源：http://hz.quarkkingdee.top/gttzeniutn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.daxiang520.top/gtnvffwcbp.html

) t WHERE rn = 1;
来源：http://hz.zhongyouzk.top/gttizqsutd.html

[Q35] 内连接
来源：http://hz.hysaishi.cn/gthmddgcws.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ivvv.top/gtsdeywucx.html

[Q36] 左连接
来源：http://hz.shzxlz.cn/gtyakdxwih.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangdashe.top/gtmplfskyh.html

[Q37] 右连接
来源：http://hz.tian-w.cn/gtaosaeydm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xuanzx.com/gtxpujmrot.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hywenlv.cn/gtxnuxofbj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinghuilouyu.cn/gtcqbxecwa.html

[Q39] 自连接（查上下级）
来源：http://hz.chenzaomai.com/gtfcfyoott.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhixingplan.top/gtdwueicfw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.pycfn.com/gthuvsrnam.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.birdmap.top/gtddozanxp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shuidangran.top/gtvbkegahr.html

[Q41] 多表连接
来源：http://hz.jinqigfzy.top/gtcgjlvlno.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gogol.net.cn/gtduorefcc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hongshengwenyu.top/gtpwuagdub.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.iojbl.cn/gtrdicrfos.html

[Q42] 连接条件附加过滤
来源：http://hz.daxiang520.top/gttdvpnlhx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yonumen.top/gtdcfyxohr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.svipenyu.cn/gtvrprpail.html

[Q43] 标量子查询
来源：http://hz.0kj1m.cn/gttkxztmyx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jiagoushi.top/gtnxhsdgyv.html

[Q44] IN 子查询
来源：http://hz.dashuyun.cn/gtxhprpqnc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xuetiantiany.cn/gtcdmqxjva.html

[Q45] EXISTS 判断存在
来源：http://hz.tanke756.top/gtbrzlajfe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gtukcxajkj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.vqdsnc.cn/gtlphbrbks.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuxming.cn/gtktjvofai.html

[Q47] 与平均值比较
来源：http://hz.guannengcc.top/gtvlpmdfow.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cashguo.top/gtbvjgxfkr.html

[Q48] CTE 公用表表达式
来源：http://hz.yj202588.top/gtcvejrvjs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhoulong.xyz/gtyrgstsut.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.aibaodan.cn/gtekjfpwcx.html

[Q49] 更新单行
来源：http://hz.hnxiangtu.top/gtjovtfibw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ppjwa.cn/gtvdqmkcsd.html

[Q50] 批量更新
来源：http://hz.jinqigfzy.top/gtafpbpsci.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.bjfxy.top/gtucqdosfl.html

[Q51] 用子查询更新
来源：http://hz.cucudq.cn/gtxvvkjauw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hongshengwenyu.top/gtjymvbcab.html

[Q52] 删除指定行
来源：http://hz.jyoumei.cn/gtrsxkxlgt.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhiwuduotai.top/gtlvhmcxup.html

[Q53] 按条件删除
来源：http://hz.jinyuanbaomall.cn/gteucjwprs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cucudq.cn/gtbgjrvbev.html

[Q54] 清空表
来源：http://hz.wangshuangyany.cn/gtfewazees.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigufen.top/gteuvzvzaj.html

[Q55] 排名（并列占位）
来源：http://hz.wangdashe.top/gtgltetpog.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yangfankeji.com/gtimwxrzjn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.9152youxi.cn/gtrhnrtaok.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhoulong.xyz/gtftxttlfp.html

[Q57] 行号
来源：http://hz.fengsongda.top/gtrygbxfhg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhiwuduotai.top/gtxllcfrwq.html

[Q58] 累计求和
来源：http://hz.daria6918.cn/gtsptgjuaa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.guannengcc.top/gtwhnrwlny.html

[Q59] 分组内累计
来源：http://hz.yueranfly.top/gtmzxggmvh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.pycfn.com/gtmvjadurw.html

[Q60] 取上一行 / 下一行
来源：http://hz.jyoumei.cn/gtqluengmm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenjidiqi.icu/gtwifomfbe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gzhubu.top/gtsmtypeqq.html

[Q61] 移动平均
来源：http://hz.aizwys.cn/gtufcahxya.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.andypj.xyz/gtyduvmonv.html

[Q62] 分组占比
来源：http://hz.snrcjt.cn/gtuvcsdobr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.dashuyun.cn/gtbkgoenlo.html

[Q63] 开启事务
来源：http://hz.yj202588.top/gtxezfqiqp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shanyushiyangkeji.top/gtvckemvby.html

[Q64] 提交事务
来源：http://hz.jiagoushi.top/gtilresblu.html

COMMIT;
来源：http://hz.9152youxi.cn/gtmvaonyex.html

[Q65] 回滚事务
来源：http://hz.haohaochexian.top/gtqumbcdli.html

ROLLBACK;
来源：http://hz.guannengcc.top/gtcojfngzn.html

[Q66] 行锁查询
来源：http://hz.cashguo.top/gtuyjspgzz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tianlin.xyz/gtfzhsmjkk.html

[Q67] 设置隔离级别
来源：http://hz.yvedp.cn/gtainweykm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yueranfly.top/gtezostacj.html

[Q68] 保存点
来源：http://hz.aibaodan.cn/gtfjcbxmmw.html

SAVEPOINT sp1;
来源：http://hz.hysaishi.cn/gttomiplvr.html

ROLLBACK TO sp1;
来源：http://hz.tian-w.cn/gtocvpmzhe.html

[Q69] 查看执行计划
来源：http://hz.zhoulong.xyz/gtudlrelsb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jqgufenzy.top/gtlgkpzfcu.html

[Q70] 更新统计信息
来源：http://hz.daria6918.cn/gtujjudftu.html

ANALYZE TABLE users;
来源：http://hz.shanyushiyangkeji.top/gtkdtwbywf.html

[Q71] 查看建表语句
来源：http://hz.wangdashe.top/gtjjwcynub.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.kuanghao11.cn/gtjrbnxuck.html

[Q72] 查看索引
来源：http://hz.yongpay.top/gtcujyinsr.html

SHOW INDEX FROM users;
来源：http://hz.tanke756.top/gtnsdlyjsu.html

[Q73] 查看表状态
来源：http://hz.ivvv.top/gtttahrwhv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.mhx1999.top/gtuqrebryv.html

[Q74] 强制使用索引
来源：http://hz.52xcode.cn/gtiaonwgih.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.iojbl.cn/gtbbchokjm.html

[Q75] 日期格式化
来源：http://hz.ybcxt.top/gtdfsbxzwz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.daria6918.cn/gtuwyekjfy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xylfe.cn/gtvkdvgdbt.html

[Q76] 按天统计
来源：http://hz.jinqigfzy.top/gticuspusb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.meibo888.top/gtvjfwuuxy.html

[Q77] 时间加减
来源：http://hz.wangdashe.top/gtgphkzplg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fengsongda.top/gtqtrlhwil.html

[Q78] 当前时间
来源：http://hz.shangyingyoupin.top/gtvjazaeud.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhongyouzk.top/gtowsunsxc.html

[Q79] 字符串拼接
来源：http://hz.daxiang520.top/gtsurgwebl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.guowangkeji.top/gtivwzohvi.html

[Q80] 字符串截取
来源：http://hz.dashuyun.cn/gtmthoshqy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinqigufen.top/gtwfgeuhva.html

[Q81] 字符串替换
来源：http://hz.xuetiantiany.cn/gttzemrsxg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.0kj1m.cn/gtzmisjeqr.html

[Q82] 字符长度与字节长度
来源：http://hz.c1oappe.top/gttctwjssj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.haohaochexian.top/gtlhzxhirh.html

[Q83] 大小写转换
来源：http://hz.yj202588.top/gtvuizzjmr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jqgfzy.top/gtkjawftdp.html

[Q84] 去除首尾空格
来源：http://hz.chenzaomai.com/gtotlftgvy.html

SELECT TRIM(name) FROM users;
来源：http://hz.quarkkingdee.top/gtqppnxsiy.html

[Q85] 数值取整
来源：http://hz.zhijiandao.cn/gtgfbryern.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yj20258.top/gtcisrdxdk.html

[Q86] 读取 JSON 字段
来源：http://hz.zhengqikj.top/gtwpifmidc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.feifeiyinyue.top/gtocuoczgs.html

[Q87] JSON 字段做条件
来源：http://hz.tanke756.top/gtqalveuqx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.smart0.xyz/gtqyqpyild.html

[Q88] 行转列（条件聚合）
来源：http://hz.316326.xyz/gtbmpkpwyo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shuidangran.top/gtgcxcwdjb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jiagoushi.top/gtzeofqvxv.html

[Q89] 判断表是否存在
来源：http://hz.zhongyouzk.top/gtzpoetssy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj20258888.top/gtfrrebmse.html

[Q90] 生成序号列
来源：http://hz.andypj.xyz/gtngpzsywh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yj202588.top/gtqhrkzplm.html

================================================================================
来源：http://hz.tian-w.cn/gtucnfdpjk.html

R. Bash 专题
来源：http://hz.hfpthk.cn/gtovbyohff.html

================================================================================
来源：http://hz.gaohongyu789.top/gtrfduizpf.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangkeji.top/gtucmhcjcx.html

#!/usr/bin/env bash
来源：http://hz.xingfuxueyuan.xyz/gtrzepozgb.html

set -euo pipefail
来源：http://hz.zhongyouzk.top/gtvrzqdfbu.html

[R02] 变量赋值与使用
来源：http://hz.ydjk.org.cn/gtlxceaqvy.html

name="Tom"; echo "$name"
来源：http://hz.hysaishi.cn/gttwmbibeb.html

[R03] 只读变量
来源：http://hz.cdnleiting.top/gthqqomsky.html

readonly PI=3.14
来源：http://hz.shangyingyoupin.top/gtgovigvwr.html

[R04] 位置参数
来源：http://hz.aizwys.cn/gtkdltgyxs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cqqwz.cn/gtoqpbszbb.html

[R05] 参数默认值
来源：http://hz.tian-w.cn/gtzeseloit.html

name="${1:-default}"
来源：http://hz.gzhubu.top/gtbiiniamh.html

[R06] 判断命令是否存在
来源：http://hz.kuanghao11.cn/gtvfbxhvqy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hammf.cn/gtpbqbjhfr.html

[R07] if 判断文件
来源：http://hz.smart0.xyz/gtelfvoccz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jqgfzy.top/gtdkpdibaw.html

[R08] 数值比较
来源：http://hz.quarkkingdee.top/gtlpsjrdvr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.iojbl.cn/gtxraviqhj.html

[R09] 字符串比较
来源：http://hz.jinyuanbaomall.cn/gtyhgrvdyh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.mhx1999.top/gtcrrzxlms.html

[R10] 正则匹配
来源：http://hz.fengsongda.top/gttbiywldv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tanke756.top/gtkrjsvzod.html

[R11] case 多分支
来源：http://hz.fzhhl.top/gtsvucgrus.html

case "$1" in
来源：http://hz.hnqzz.top/gtpvspiouw.html

start) echo "启动" ;;
来源：http://hz.shuidangran.top/gtdbyywcgq.html

stop)  echo "停止" ;;
来源：http://hz.jqgufenzy.top/gtkmfsbvnp.html

*)     echo "未知命令" ;;
来源：http://hz.yj20258.top/gtcjdljgac.html

esac
来源：http://hz.cqqwz.cn/gtrvhlszlr.html

[R12] for 遍历文件
来源：http://hz.gaohongyu789.top/gtxlhwamsm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.pengpengdd.cyou/gtebejixan.html

[R13] for 计数循环
来源：http://hz.aibaodan.cn/gttphcnqtw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ehwqpu.com/gtkfkailvy.html

[R14] C 风格 for
来源：http://hz.zhixingplan.top/gtnvgsshdg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nanxuanxn.top/gtjeimkzqq.html

[R15] while 逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtxudsljof.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.wangshuangyany.cn/gtenuztpod.html

[R16] until 等待条件
来源：http://hz.xuetiantiany.cn/gtmnwetbwg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hnqzz.top/gtsnfyqudk.html

[R17] 数组定义与取值
来源：http://hz.aizwys.cn/gtizoxgpsw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aizwys.cn/gtzfjkrjki.html

[R18] 遍历数组
来源：http://hz.chenzaomai.com/gtmswqzurd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangtech.top/gtfnygewdb.html

[R19] 数组长度
来源：http://hz.snrcjt.cn/gtpeswktln.html

echo "${#arr[@]}"
来源：http://hz.ydzc1.top/gtkcwsvzfj.html

[R20] 关联数组（字典）
来源：http://hz.sxryk.cn/gtvoqezlyx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ppjwa.cn/gtwwysxwvo.html

[R21] 字符串长度
来源：http://hz.sysykeji.top/gtywzyxane.html

echo "${#s}"
来源：http://hz.gzhubu.top/gtjobejaed.html

[R22] 截取子串
来源：http://hz.haohaochexian.top/gtqivmketr.html

echo "${s:0:5}"
来源：http://hz.hfpthk.cn/gtxudkdpsa.html

[R23] 字符串替换
来源：http://hz.svipenyu.cn/gtiiczsklr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.9152youxi.cn/gtzhjdguvb.html

[R24] 大小写转换
来源：http://hz.zdqjudy.top/gtyuscnycz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.9152youxi.cn/gtopylxkse.html

[R25] 去后缀 / 去前缀
来源：http://hz.yanxiufei.cn/gtxhmcaatm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jqgfzy.top/gtudthbnip.html

[R26] 命令替换
来源：http://hz.ywan-chungtsiang.top/gtosypqbks.html

now=$(date +%F); echo "$now"
来源：http://hz.hnqzz.top/gtllsdzqta.html

[R27] 算术展开
来源：http://hz.9152youxi.cn/gtiualctkr.html

echo $((1 + 2 * 3))
来源：http://hz.9152youxi.cn/gtwwmqpceb.html

[R28] 浮点运算
来源：http://hz.chenlongwang.top/gtrlmrmact.html

echo "scale=2; 10/3" | bc
来源：http://hz.xinyue.icu/gtrfiimgzg.html

[R29] 定义函数
来源：http://hz.jiagoushi.top/gtrcvajhpw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.kuanghao11.cn/gtgyyhrznr.html

[R30] 函数返回状态码
来源：http://hz.0kj1m.cn/gtgukcggve.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.feifeiyinyue.top/gtldvqusgu.html

[R31] 局部变量
来源：http://hz.birdmap.top/gtbgykprqq.html

f() { local x=1; echo "$x"; }
来源：http://hz.shanyushiyangtech.top/gtcadmzygo.html

[R32] 参数个数校验
来源：http://hz.jinqigufen.top/gthgdtdimy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.wangshuangyany.cn/gtbvibghsw.html

[R33] 捕获错误并提示行号
来源：http://hz.cucudq.cn/gtmyfjxnni.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jlsjyb.cn/gtpiezugkv.html

[R34] 退出时清理
来源：http://hz.zdqjudy.top/gtgppwkqgt.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.iojbl.cn/gtrkvpdxtu.html

[R35] 后台执行并等待
来源：http://hz.yvedp.cn/gtnsvrkwic.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.nanxinkj.top/gtiypcgzhn.html

[R36] 并发执行多个任务
来源：http://hz.zhiwuduotai.top/gtpamkweus.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenlongwang.top/gtjqvmljlj.html

[R37] 把输出赋给变量
来源：http://hz.sweek.top/gtgnifvuxg.html

files=$(ls -1)
来源：http://hz.snrcjt.cn/gtcysexkvk.html

[R38] 管道串联
来源：http://hz.daria6918.cn/gtvinhwuyd.html

cat a.txt | grep -i error | wc -l
来源：http://hz.aizwys.cn/gtnulrluxk.html

[R39] 重定向标准输出与错误
来源：http://hz.jinqigufen.top/gtyesvipkt.html

cmd > out.log 2>&1
来源：http://hz.sufxvd.cn/gtzvakyzwl.html

[R40] 追加写日志
来源：http://hz.cucudq.cn/gtwbxmqzyv.html

echo "log" >> out.log
来源：http://hz.zhengqikj.top/gtvsnrzzmz.html

[R41] 丢弃输出
来源：http://hz.aibaodan.cn/gtsxtvcfue.html

cmd >/dev/null 2>&1
来源：http://hz.hammf.cn/gtykpqzcxt.html

[R42] 输入重定向
来源：http://hz.cqqwz.cn/gtynagqimu.html

wc -l < a.txt
来源：http://hz.birdmap.top/gtrxnztjib.html

[R43] 按名字查找文件
来源：http://hz.shangyingyoupin.top/gtqtfywxzl.html

find . -name "*.log" -type f
来源：http://hz.guannengcc.top/gtrtqnvznu.html

[R44] 按修改时间查找
来源：http://hz.cucudq.cn/gtssclkahf.html

find . -mtime -7 -type f
来源：http://hz.cashguo.top/gtmctgfmiw.html

[R45] 批量删除
来源：http://hz.quarkkingdee.top/gtnphdhfyb.html

find . -name "*.tmp" -delete
来源：http://hz.xinyue.icu/gtohxvthpi.html

[R46] 递归替换文件内容
来源：http://hz.jianghu66.top/gtlytxdtvo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhoulong.xyz/gtbpdaqfav.html

[R47] sed 单行替换
来源：http://hz.hongshengwenyu.top/gtorazcyxk.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.feifeiyinyue.top/gtkbjpogfn.html

[R48] awk 取指定列
来源：http://hz.316326.xyz/gtpcatjcys.html

awk '{print $1, $3}' a.txt
来源：http://hz.hammf.cn/gtfaovdgzw.html

[R49] awk 带条件
来源：http://hz.yj20258.top/gtcgudkqhk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.fengsongda.top/gtvelqecvv.html

[R50] awk 求和
来源：http://hz.ydzc1.top/gtyakkkuzc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yvedp.cn/gtchwdadaw.html

[R51] 排序去重取前几
来源：http://hz.ivvv.top/gtpixwjnvx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.kuanghao11.cn/gtbgymagst.html

[R52] 统计行数
来源：http://hz.ydzc1.top/gtchudazgn.html

wc -l a.txt
来源：http://hz.aizwys.cn/gtxjpainma.html

[R53] 查看文件头与实时尾
来源：http://hz.fzhhl.top/gtjwvcazjg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinqigufen.top/gtrehgdxee.html

[R54] 比较两个文件
来源：http://hz.pycfn.com/gtcmhgavrs.html

diff a.txt b.txt
来源：http://hz.zhoulong.xyz/gtgnrlpboo.html

[R55] 压缩与解压
来源：http://hz.nanxinkj.top/gtuhwqlgvu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sweek.top/gtxeaxjzhd.html

[R56] 远程拷贝
来源：http://hz.bjfxy.top/gtldtvfoyh.html

scp file user@host:/path/
来源：http://hz.cqqwz.cn/gtbsbaarkr.html

[R57] 远程执行命令
来源：http://hz.andypj.xyz/gtbbgkzakj.html

ssh user@host 'uptime'
来源：http://hz.yuxming.cn/gtsxrjqoro.html

[R58] 下载文件
来源：http://hz.shangyingyoupin.top/gtiszluatj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cdnleiting.top/gtyznxvsjk.html

[R59] 发 POST JSON
来源：http://hz.tanke756.top/gtahdifysg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhoulong.xyz/gtxksoktib.html

[R60] 只看 HTTP 状态码
来源：http://hz.cqqwz.cn/gtdfurpdiz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhaomingkeji.xyz/gtgockhnqp.html

[R61] 磁盘占用
来源：http://hz.nanxuanxn.top/gthplpsdqg.html

df -h;  du -sh *
来源：http://hz.xylfe.cn/gtgxguigez.html

[R62] 找最占空间的文件
来源：http://hz.yj20258.top/gtqnxxvzcb.html

du -ah . | sort -rh | head -10
来源：http://hz.wangshuangyany.cn/gtqhockkhf.html

[R63] 内存与进程
来源：http://hz.dashuyun.cn/gtlvebnlla.html

free -h;  ps aux | grep nginx
来源：http://hz.ywan-chungtsiang.top/gtejcmlqwo.html

[R64] 结束进程
来源：http://hz.shangyingyoupin.top/gtuylbobyd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gzhubu.top/gtewxnkvhd.html

[R65] 查看端口占用
来源：http://hz.snrcjt.cn/gteiugnvgv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xylfe.cn/gtweaujmjw.html

[R66] 定时任务
来源：http://hz.yuxming.cn/gtkkfygjlo.html

crontab -e;  crontab -l
来源：http://hz.nanxinkj.top/gtbdtykuzo.html

[R67] 生成随机十六进制串
来源：http://hz.ybcxt.top/gtsstmahfz.html

openssl rand -hex 16
来源：http://hz.jqgufenzy.top/gtqscoeagm.html

[R68] 计算文件校验值
来源：http://hz.kuanghao11.cn/gtjrejoget.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cdnleiting.top/gtzbwuncly.html

[R69] 生成随机密码
来源：http://hz.guannengcc.top/gtdyulokbd.html

head -c 16 /dev/urandom | base64
来源：http://hz.daria6918.cn/gturucovqa.html

[R70] 时间戳与互转
来源：http://hz.zhongyouzk.top/gtbyenxopc.html

date +%s;  date -d @1700000000
来源：http://hz.shzxlz.cn/gtbpgidivp.html

[R71] 日期格式化
来源：http://hz.hysaishi.cn/gtnawvboyc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yj20258.top/gtmlqtmgkr.html

[R72] 等待端口就绪
来源：http://hz.nwbrower.top/gtnluckryl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gtjsumeqiz.html

[R73] 分割大日志
来源：http://hz.jyoumei.cn/gtpcvpykms.html

split -l 1000 big.log part_
来源：http://hz.pycfn.com/gtanhulmav.html

[R74] 批量重命名
来源：http://hz.zhixingplan.top/gtcxlzvrfn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xingfuxueyuan.xyz/gtxnbkluuv.html

[R75] 导出环境变量
来源：http://hz.ydjk.org.cn/gtqbszrjri.html


<!-- 参考信息 -->