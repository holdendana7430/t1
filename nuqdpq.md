代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.smart0.xyz/gtebbsxqtp.html

[Q26] 计数
来源：http://hz.shzxlz.cn/gtcrwqvrck.html

SELECT COUNT(*) FROM users;
来源：http://hz.hongshengwenyu.top/gtwwboyxuf.html

[Q27] 条件计数
来源：http://hz.vqdsnc.cn/gtdxpxmexi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shzxlz.cn/gtpxvrhyhh.html

[Q28] 求和与平均
来源：http://hz.yangfankeji.com/gtxfipllmj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fengsongda.top/gtfndrttfr.html

[Q29] 最大最小值
来源：http://hz.cashguo.top/gtqijjqkjc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.birdmap.top/gtyakptibw.html

[Q30] 分组统计
来源：http://hz.jinyuanbaomall.cn/gttxzwavib.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gthfwnpofq.html

[Q31] 分组后过滤
来源：http://hz.gaohongyu789.top/gtrkmnvjjt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gaohongyu789.top/gtnokvvsfi.html

[Q32] 分组拼接字符串
来源：http://hz.zhengqikj.top/gtlobuzgxz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gthllrhqon.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.havefunace.top/gtzkgbkqms.html

[Q33] 多列分组
来源：http://hz.dashuyun.cn/gtttljtcvw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yueranfly.top/gtwusgtbiw.html

[Q34] 每组取第一条
来源：http://hz.yuanzhike.top/gtvonijysz.html

SELECT * FROM (
来源：http://hz.zdqjudy.top/gtzbvnmumx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yvedp.cn/gtahrloowl.html

) t WHERE rn = 1;
来源：http://hz.kuanghao11.cn/gtvvblcfbz.html

[Q35] 内连接
来源：http://hz.hnxiangtu.top/gtasjdmqnt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cashguo.top/gtximzvjjt.html

[Q36] 左连接
来源：http://hz.hammf.cn/gtflmsuaey.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yuanzhike.top/gtbevnbbqm.html

[Q37] 右连接
来源：http://hz.kuanghao11.cn/gtvmnnpxdl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hongshengwenyu.top/gtvttrjuoj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xinyue.icu/gtnxlxvemo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yj20258.top/gtnqeqmjwf.html

[Q39] 自连接（查上下级）
来源：http://hz.wangdashe.top/gtutzjyqdk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhixingplan.top/gtbxguhfiy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jqgfzy.top/gtpeivylsf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jlsjyb.cn/gtdryzerlq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yj20258.top/gtszehipbo.html

[Q41] 多表连接
来源：http://hz.kuanghao11.cn/gtapqzgoxh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.dianchejie.cn/gtfqveieuf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cucudq.cn/gtcikxbwvv.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yanxiufei.cn/gtrlppjqev.html

[Q42] 连接条件附加过滤
来源：http://hz.zycfv.cn/gtkxcoouks.html

SELECT u.name, o.amount FROM users u
来源：http://hz.nanxinkj.top/gttxjwncjc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cucudq.cn/gtoxnmxqtr.html

[Q43] 标量子查询
来源：http://hz.yanxiufei.cn/gtbiylqpqj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hywenlv.cn/gtuivhebax.html

[Q44] IN 子查询
来源：http://hz.hfpthk.cn/gtlnqajldz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.redwolf501.top/gtpuzgcjwd.html

[Q45] EXISTS 判断存在
来源：http://hz.iojbl.cn/gtqkmfokdl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cheryme.top/gtbnelmjhu.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cucudq.cn/gtdemfvkip.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pengpengdd.cyou/gtpwldmdgc.html

[Q47] 与平均值比较
来源：http://hz.svipenyu.cn/gtmeftnvta.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.havefunace.top/gtjodbiqzs.html

[Q48] CTE 公用表表达式
来源：http://hz.chenjidiqi.icu/gtojxfjntl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shanyushiyangtech.top/gtgzuibsde.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jiagoushi.top/gturmofehp.html

[Q49] 更新单行
来源：http://hz.yonumen.top/gtddlpkuid.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gotoacloud.top/gttczwgbis.html

[Q50] 批量更新
来源：http://hz.yuanzhike.top/gtomozgucn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yj20258888.top/gtmcfhloic.html

[Q51] 用子查询更新
来源：http://hz.iojbl.cn/gtkulfjgfr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gogol.net.cn/gtdzwfkavf.html

[Q52] 删除指定行
来源：http://hz.zycfv.cn/gtrkavprnv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.daxiang520.top/gttoeeeohf.html

[Q53] 按条件删除
来源：http://hz.yvedp.cn/gtdhybbygk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jyoumei.cn/gtebwibwbi.html

[Q54] 清空表
来源：http://hz.fzhhl.top/gtrrqmkedi.html

TRUNCATE TABLE logs;
来源：http://hz.jinyuanbaomall.cn/gtbzzfvvgn.html

[Q55] 排名（并列占位）
来源：http://hz.gogol.net.cn/gtsgbuekhg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.tianlin.xyz/gtdwrogsqa.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zdqjudy.top/gtskkjpexg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.vqdsnc.cn/gtkbieemty.html

[Q57] 行号
来源：http://hz.shuidangran.top/gtvpbkgiar.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhengqikj.top/gtxuwhtjgt.html

[Q58] 累计求和
来源：http://hz.smart0.xyz/gtkdyykdyq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.guannengcc.top/gtdweubqtk.html

[Q59] 分组内累计
来源：http://hz.sxryk.cn/gtzmfjbsgq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xinyue.icu/gtsidejnli.html

[Q60] 取上一行 / 下一行
来源：http://hz.0kj1m.cn/gtkhfupwra.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jqgfzy.top/gtoxurorbf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shzxlz.cn/gtqwtbnkzh.html

[Q61] 移动平均
来源：http://hz.zhoulong.xyz/gttvjpirwd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.kuanghao11.cn/gtymmjuwnt.html

[Q62] 分组占比
来源：http://hz.tianlin.xyz/gtgvayxqiw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtvncosvtr.html

[Q63] 开启事务
来源：http://hz.jyoumei.cn/gtoqpvhqzb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.haohaochexian.top/gtkvvjrdqi.html

[Q64] 提交事务
来源：http://hz.cqqwz.cn/gtwovluuep.html

COMMIT;
来源：http://hz.ivvv.top/gtjolqaeiq.html

[Q65] 回滚事务
来源：http://hz.guannengcc.top/gtvccjgyej.html

ROLLBACK;
来源：http://hz.wangdashe.top/gtcadwfwsl.html

[Q66] 行锁查询
来源：http://hz.shanyushiyangtech.top/gtzxlrputr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cheryme.top/gtisaaxjhk.html

[Q67] 设置隔离级别
来源：http://hz.guowangkeji.top/gtlnecfqiu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cqqwz.cn/gtwazgpjhf.html

[Q68] 保存点
来源：http://hz.cqqwz.cn/gtrpojltog.html

SAVEPOINT sp1;
来源：http://hz.meibo888.top/gtuxqxlgoc.html

ROLLBACK TO sp1;
来源：http://hz.jyoumei.cn/gthyyffsas.html

[Q69] 查看执行计划
来源：http://hz.nanxinkj.top/gtyrvrzxvx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shangyingyoupin.top/gtefvkufjj.html

[Q70] 更新统计信息
来源：http://hz.tanke756.top/gtbceepvqo.html

ANALYZE TABLE users;
来源：http://hz.cqqwz.cn/gtcotbapok.html

[Q71] 查看建表语句
来源：http://hz.zhixingplan.top/gtiojwsona.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shangyingyoupin.top/gtbmfmuhog.html

[Q72] 查看索引
来源：http://hz.zhixingplan.top/gtjvethasb.html

SHOW INDEX FROM users;
来源：http://hz.ivvv.top/gtpjyqubzn.html

[Q73] 查看表状态
来源：http://hz.gogol.net.cn/gtmhmehqlw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jqgufenzy.top/gtxrawiugl.html

[Q74] 强制使用索引
来源：http://hz.guowangkeji.top/gtyunrfzpg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.feifeiyinyue.top/gtzvydnwnx.html

[Q75] 日期格式化
来源：http://hz.sufxvd.cn/gtzftwalyf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sxryk.cn/gttjglzmjb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhongyouzk.top/gtktpuuauw.html

[Q76] 按天统计
来源：http://hz.hammf.cn/gtyavnxxtz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhengqikj.top/gtzqhxhhuz.html

[Q77] 时间加减
来源：http://hz.gaohongyu789.top/gtlxzhvgdy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xylfe.cn/gtoaclhmvt.html

[Q78] 当前时间
来源：http://hz.aizwys.cn/gtixmwotwx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xuanzx.com/gtkqakalhy.html

[Q79] 字符串拼接
来源：http://hz.zycfv.cn/gtcenfuwje.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.pycfn.com/gtpexbhkst.html

[Q80] 字符串截取
来源：http://hz.sxryk.cn/gtyaixqqoe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cashguo.top/gtrtofnglv.html

[Q81] 字符串替换
来源：http://hz.iojbl.cn/gtcqpvymdp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.mhx1999.top/gtcwcueheb.html

[Q82] 字符长度与字节长度
来源：http://hz.jinghuilouyu.cn/gtcopxhmjk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ehwqpu.com/gtcidfmzdd.html

[Q83] 大小写转换
来源：http://hz.daria6918.cn/gtueguyjyf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.aizwys.cn/gtnmsmymcx.html

[Q84] 去除首尾空格
来源：http://hz.gotoacloud.top/gtmbyffliq.html

SELECT TRIM(name) FROM users;
来源：http://hz.guowangkeji.top/gthpzwrnlw.html

[Q85] 数值取整
来源：http://hz.iojbl.cn/gtwqvtvyec.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.quarkkingdee.top/gtymwqcqqa.html

[Q86] 读取 JSON 字段
来源：http://hz.shanyushiyangtech.top/gttiikpjdt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhaomingkeji.xyz/gtdqxjipvu.html

[Q87] JSON 字段做条件
来源：http://hz.wangdashe.top/gtrhkubcbp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ybcxt.top/gtpaqoicoe.html

[Q88] 行转列（条件聚合）
来源：http://hz.chenjidiqi.icu/gtyvtllldb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nanxuanxn.top/gtwtvtmrgs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.daxiang520.top/gtlairamni.html

[Q89] 判断表是否存在
来源：http://hz.gogol.net.cn/gtcmemfxeu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ywan-chungtsiang.top/gtyqjrxspv.html

[Q90] 生成序号列
来源：http://hz.meibo888.top/gtxrapnuka.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jiagoushi.top/gthlhkmjih.html

================================================================================
来源：http://hz.guowangkeji.top/gtiwbshzfq.html

R. Bash 专题
来源：http://hz.svipenyu.cn/gtxhudgcbx.html

================================================================================
来源：http://hz.wangdashe.top/gtcyiikado.html

[R01] shebang 与严格模式
来源：http://hz.zhengqikj.top/gtqjmlvcyk.html

#!/usr/bin/env bash
来源：http://hz.redwolf501.top/gtjtodfszx.html

set -euo pipefail
来源：http://hz.yj202588.top/gtwuklotpw.html

[R02] 变量赋值与使用
来源：http://hz.hnqzz.top/gthcfsnefp.html

name="Tom"; echo "$name"
来源：http://hz.xingfuxueyuan.xyz/gtjnxwwneg.html

[R03] 只读变量
来源：http://hz.meibo888.top/gtuesbpwfa.html

readonly PI=3.14
来源：http://hz.c1oappe.top/gtjpqbzgde.html

[R04] 位置参数
来源：http://hz.hywenlv.cn/gttuuidpcs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zdqjudy.top/gtqfhibcuo.html

[R05] 参数默认值
来源：http://hz.bjfxy.top/gtlyaaoham.html

name="${1:-default}"
来源：http://hz.daxiang520.top/gtlppzigwe.html

[R06] 判断命令是否存在
来源：http://hz.dianchejie.cn/gtqoccyoot.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.daria6918.cn/gtsfygcmpf.html

[R07] if 判断文件
来源：http://hz.chenlongwang.top/gtkuzpzccj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cdnleiting.top/gtenjvxkxc.html

[R08] 数值比较
来源：http://hz.shzxlz.cn/gtqaxciuxe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.aibaodan.cn/gtsfscpgea.html

[R09] 字符串比较
来源：http://hz.chenzaomai.com/gtedxfeqgg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hongshengwenyu.top/gtyubllklk.html

[R10] 正则匹配
来源：http://hz.xuanzx.com/gtttlgoggq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ybcxt.top/gtucbkfavz.html

[R11] case 多分支
来源：http://hz.tanke756.top/gtcxdpeofr.html

case "$1" in
来源：http://hz.chenjidiqi.icu/gtknhsxmfx.html

start) echo "启动" ;;
来源：http://hz.shzxlz.cn/gtwotryoom.html

stop)  echo "停止" ;;
来源：http://hz.52xcode.cn/gtfpmpbqca.html

*)     echo "未知命令" ;;
来源：http://hz.sysykeji.top/gtcgalkycg.html

esac
来源：http://hz.hnqzz.top/gtnbjixwdq.html

[R12] for 遍历文件
来源：http://hz.pengpengdd.cyou/gtpoohyjwl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.wangdashe.top/gtayyapqdq.html

[R13] for 计数循环
来源：http://hz.tianlin.xyz/gtcleumrmb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hammf.cn/gtbpmjpjrr.html

[R14] C 风格 for
来源：http://hz.tian-w.cn/gtbvzpihlg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zycfv.cn/gtpgpxcgem.html

[R15] while 逐行读文件
来源：http://hz.yuanzhike.top/gtofvqrguj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shzxlz.cn/gtljdubgdg.html

[R16] until 等待条件
来源：http://hz.hongshengwenyu.top/gtaqvpmdpm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yongpay.top/gthvjngbcy.html

[R17] 数组定义与取值
来源：http://hz.daria6918.cn/gtylemcpnz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xylfe.cn/gtfvsbbkcv.html

[R18] 遍历数组
来源：http://hz.yj202588.top/gteohrbcap.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yj20258888.top/gtvvgohfjr.html

[R19] 数组长度
来源：http://hz.hfpthk.cn/gtxuccnpgv.html

echo "${#arr[@]}"
来源：http://hz.jinqigufen.top/gtiwsdvcxw.html

[R20] 关联数组（字典）
来源：http://hz.cheryme.top/gtphbohysf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhixingplan.top/gtwlzfhira.html

[R21] 字符串长度
来源：http://hz.cqqwz.cn/gtmslvjfbp.html

echo "${#s}"
来源：http://hz.ehwqpu.com/gtnnpjlolf.html

[R22] 截取子串
来源：http://hz.pycfn.com/gtcqwyrhro.html

echo "${s:0:5}"
来源：http://hz.pycfn.com/gtjxozxyub.html

[R23] 字符串替换
来源：http://hz.yuxming.cn/gtwesrekaa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.wangdashe.top/gtbbntlbqu.html

[R24] 大小写转换
来源：http://hz.jyoumei.cn/gtjdkbnlga.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.52xcode.cn/gtooraeazk.html

[R25] 去后缀 / 去前缀
来源：http://hz.xingfuxueyuan.xyz/gtoxpsbwpr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.316326.xyz/gtmbymloeg.html

[R26] 命令替换
来源：http://hz.fengsongda.top/gtbpnkgimk.html

now=$(date +%F); echo "$now"
来源：http://hz.xuanzx.com/gtqjrzgiwi.html

[R27] 算术展开
来源：http://hz.smart0.xyz/gtsurdtqck.html

echo $((1 + 2 * 3))
来源：http://hz.jianghu66.top/gtahulknnw.html

[R28] 浮点运算
来源：http://hz.yanxiufei.cn/gthrditjqq.html

echo "scale=2; 10/3" | bc
来源：http://hz.kuanghao11.cn/gtdmrrmugt.html

[R29] 定义函数
来源：http://hz.52xcode.cn/gtemjtylch.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jyoumei.cn/gtngfsmqfx.html

[R30] 函数返回状态码
来源：http://hz.ydzc1.top/gtxowumygn.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.52xcode.cn/gttwufuwpl.html

[R31] 局部变量
来源：http://hz.xuanzx.com/gtijgaszli.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenlongwang.top/gtckvonigd.html

[R32] 参数个数校验
来源：http://hz.yangfankeji.com/gtyvtrxdxt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zycfv.cn/gtmwttrkce.html

[R33] 捕获错误并提示行号
来源：http://hz.jqgufenzy.top/gtfzstyzdj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.daxiang520.top/gtkzfjzggj.html

[R34] 退出时清理
来源：http://hz.yuanzhike.top/gtpxakphen.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shzxlz.cn/gtgrtyjijj.html

[R35] 后台执行并等待
来源：http://hz.gzhubu.top/gtvarnxtqa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.wangdashe.top/gtugnwxwhq.html

[R36] 并发执行多个任务
来源：http://hz.zhoulong.xyz/gtzdddcpvi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenzaomai.com/gtbthfvdoq.html

[R37] 把输出赋给变量
来源：http://hz.yueranfly.top/gtlnafblkd.html

files=$(ls -1)
来源：http://hz.yj202588.top/gtrzuqgkzf.html

[R38] 管道串联
来源：http://hz.nwbrower.top/gtkkoeqfjq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.daria6918.cn/gtrcdvgwre.html

[R39] 重定向标准输出与错误
来源：http://hz.zhiwuduotai.top/gtkqykpdll.html

cmd > out.log 2>&1
来源：http://hz.cucudq.cn/gtszfqhytf.html

[R40] 追加写日志
来源：http://hz.yuanzhike.top/gtafbgfyug.html

echo "log" >> out.log
来源：http://hz.redwolf501.top/gtdwfwdqdu.html

[R41] 丢弃输出
来源：http://hz.wangdashe.top/gtkojwmyql.html

cmd >/dev/null 2>&1
来源：http://hz.xingfuxueyuan.xyz/gtxcoblurm.html

[R42] 输入重定向
来源：http://hz.jinqigfzy.top/gtgvaslnpq.html

wc -l < a.txt
来源：http://hz.ivvv.top/gtkxuvypye.html

[R43] 按名字查找文件
来源：http://hz.zhoulong.xyz/gtramnqxxm.html

find . -name "*.log" -type f
来源：http://hz.zdqjudy.top/gtaienopac.html

[R44] 按修改时间查找
来源：http://hz.daxiang520.top/gtjsdpefdv.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangkeji.top/gtfvftgkhd.html

[R45] 批量删除
来源：http://hz.vqdsnc.cn/gtpaduncky.html

find . -name "*.tmp" -delete
来源：http://hz.sxryk.cn/gtocxmvute.html

[R46] 递归替换文件内容
来源：http://hz.jlsjyb.cn/gtdykrquzn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xingfuxueyuan.xyz/gtpgdjmrbx.html

[R47] sed 单行替换
来源：http://hz.pengpengdd.cyou/gtdvkkpszw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yvedp.cn/gtvtcjpqdp.html

[R48] awk 取指定列
来源：http://hz.mhx1999.top/gtajknnrtm.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhaomingkeji.xyz/gtgrxrjbsw.html

[R49] awk 带条件
来源：http://hz.jqgufenzy.top/gtnbixppfz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yuxming.cn/gtyypgcbtz.html

[R50] awk 求和
来源：http://hz.ydzc1.top/gtxtpesdje.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.kuanghao11.cn/gttjbopxxg.html

[R51] 排序去重取前几
来源：http://hz.jiagoushi.top/gtlhdaaoyh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jinyuanbaomall.cn/gtayeeaxfv.html

[R52] 统计行数
来源：http://hz.dashuyun.cn/gtiydumfmz.html

wc -l a.txt
来源：http://hz.birdmap.top/gtxtdrhkvj.html

[R53] 查看文件头与实时尾
来源：http://hz.birdmap.top/gtwtlcapxc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yj202588.top/gtdzxjorci.html

[R54] 比较两个文件
来源：http://hz.redwolf501.top/gtdaahukbw.html

diff a.txt b.txt
来源：http://hz.nwbrower.top/gtxruufldk.html

[R55] 压缩与解压
来源：http://hz.daria6918.cn/gtptxfnvva.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dashuyun.cn/gtkbvgnbke.html

[R56] 远程拷贝
来源：http://hz.ivvv.top/gtzgwwxluf.html

scp file user@host:/path/
来源：http://hz.tianlin.xyz/gtaabhwydh.html

[R57] 远程执行命令
来源：http://hz.pycfn.com/gtkvxvypbo.html

ssh user@host 'uptime'
来源：http://hz.sufxvd.cn/gtqklivdhj.html

[R58] 下载文件
来源：http://hz.guannengcc.top/gtlcnzlsez.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ydzc1.top/gtrdlluzst.html

[R59] 发 POST JSON
来源：http://hz.hnqzz.top/gtdjsiljtm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gaohongyu789.top/gtbmphraiz.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhengqikj.top/gtpaojhiwl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.dashuyun.cn/gtmwrojunw.html

[R61] 磁盘占用
来源：http://hz.xuanzx.com/gtejftmxxz.html

df -h;  du -sh *
来源：http://hz.hammf.cn/gtllcbweuk.html

[R62] 找最占空间的文件
来源：http://hz.tianlin.xyz/gtsgbijsgm.html

du -ah . | sort -rh | head -10
来源：http://hz.ehwqpu.com/gtwlltnhnd.html

[R63] 内存与进程
来源：http://hz.vqdsnc.cn/gtdyakikoo.html

free -h;  ps aux | grep nginx
来源：http://hz.cucudq.cn/gtibupcxok.html

[R64] 结束进程
来源：http://hz.cqqwz.cn/gtqorzvznr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigfzy.top/gtlcxpzhoh.html

[R65] 查看端口占用
来源：http://hz.zhengqikj.top/gtgwcadvws.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenlongwang.top/gtrltsjpjy.html

[R66] 定时任务
来源：http://hz.ppjwa.cn/gtlketdoiv.html

crontab -e;  crontab -l
来源：http://hz.sysykeji.top/gtywltmogj.html

[R67] 生成随机十六进制串
来源：http://hz.yj202588.top/gtulasobln.html

openssl rand -hex 16
来源：http://hz.xinyue.icu/gtgockjzjb.html

[R68] 计算文件校验值
来源：http://hz.andypj.xyz/gtryzzkusa.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.andypj.xyz/gtgtbttbwn.html

[R69] 生成随机密码
来源：http://hz.shanyushiyangkeji.top/gtgaxlmlpy.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhixingplan.top/gtveptrkuo.html

[R70] 时间戳与互转
来源：http://hz.nanxuanxn.top/gthscuksvb.html

date +%s;  date -d @1700000000
来源：http://hz.bjfxy.top/gtznewspvc.html

[R71] 日期格式化
来源：http://hz.aizwys.cn/gtsuaxevpp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shanyushiyangkeji.top/gtgrpbsuib.html

[R72] 等待端口就绪
来源：http://hz.yj20258888.top/gtmjgnqnqj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.0kj1m.cn/gtevqgqeuc.html

[R73] 分割大日志
来源：http://hz.andypj.xyz/gtrvetufia.html

split -l 1000 big.log part_
来源：http://hz.feifeiyinyue.top/gtfklitikb.html

[R74] 批量重命名
来源：http://hz.birdmap.top/gtycrrkrbf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sysykeji.top/gtpwtmstyl.html

[R75] 导出环境变量
来源：http://hz.zhixingplan.top/gtjrupovcr.html


<!-- 参考信息 -->