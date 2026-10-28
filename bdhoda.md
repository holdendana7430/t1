代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.9152youxi.cn/gtkafqdvfo.html

[Q28] 求和与平均
来源：http://hz.zhengqikj.top/gtawbnitsq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.chenjidiqi.icu/gtaemvprrg.html

[Q29] 最大最小值
来源：http://hz.cqqwz.cn/gtkzksnogt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.guannengcc.top/gtagccojml.html

[Q30] 分组统计
来源：http://hz.sxryk.cn/gtmpnuvzoq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinqigufen.top/gtroyvuaau.html

[Q31] 分组后过滤
来源：http://hz.haohaochexian.top/gtqryvbqor.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.aibaodan.cn/gtiukswkxl.html

[Q32] 分组拼接字符串
来源：http://hz.sysykeji.top/gtvgffpypj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtcsqqyxqg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.0kj1m.cn/gtqtqzxumi.html

[Q33] 多列分组
来源：http://hz.xylfe.cn/gtduwtpkff.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.mhx1999.top/gtpuhnupbo.html

[Q34] 每组取第一条
来源：http://hz.gotoacloud.top/gtzaeaqodu.html

SELECT * FROM (
来源：http://hz.hongshengwenyu.top/gteooqmehy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hysaishi.cn/gtenmtjmom.html

) t WHERE rn = 1;
来源：http://hz.birdmap.top/gtjumgxyzv.html

[Q35] 内连接
来源：http://hz.birdmap.top/gtwlqtjdvm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.316326.xyz/gtsuntdvds.html

[Q36] 左连接
来源：http://hz.zhiwuduotai.top/gtmvjrtqtt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj202588.top/gtagxziwpn.html

[Q37] 右连接
来源：http://hz.dianchejie.cn/gtcdvcrxbp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.guannengcc.top/gtsvmeqmps.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xinyue.icu/gtxrxxfeej.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gotoacloud.top/gtbsvpgnql.html

[Q39] 自连接（查上下级）
来源：http://hz.hywenlv.cn/gteaadeeqx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gzhubu.top/gtzqewhmzc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.wangdashe.top/gtqazjfjmi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.tian-w.cn/gtbmbtolsy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gogol.net.cn/gtomrwkflp.html

[Q41] 多表连接
来源：http://hz.yj202588.top/gtdyjcuscu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gzhubu.top/gtkamtmlog.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hnqzz.top/gtmryiilmf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jlsjyb.cn/gtioebpwcc.html

[Q42] 连接条件附加过滤
来源：http://hz.zhixingplan.top/gtfqnusjwd.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cucudq.cn/gtjsezhanm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgufenzy.top/gtvvqvclve.html

[Q43] 标量子查询
来源：http://hz.sufxvd.cn/gtwsoqtleo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ehwqpu.com/gtvdphlglo.html

[Q44] IN 子查询
来源：http://hz.c1oappe.top/gtwmrknmvs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.pycfn.com/gtlgublrgd.html

[Q45] EXISTS 判断存在
来源：http://hz.cqqwz.cn/gtmcgcsckc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangshuangyany.cn/gtvhcbkyit.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.wangdashe.top/gtqogcqkqq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cashguo.top/gtagwugfni.html

[Q47] 与平均值比较
来源：http://hz.yj20258.top/gtrjkcvcac.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yueranfly.top/gtwaqjqfhz.html

[Q48] CTE 公用表表达式
来源：http://hz.hongshengwenyu.top/gtrlrjpqnf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhengqikj.top/gtfwqlulfp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zycfv.cn/gtdchbbunu.html

[Q49] 更新单行
来源：http://hz.yuanzhike.top/gtafnmfmsv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yuxming.cn/gtjcwyonqn.html

[Q50] 批量更新
来源：http://hz.vqdsnc.cn/gtdiqusysu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinyuanbaomall.cn/gtvcxydydl.html

[Q51] 用子查询更新
来源：http://hz.aizwys.cn/gtnwxmfyuo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cheryme.top/gtklgvbull.html

[Q52] 删除指定行
来源：http://hz.hysaishi.cn/gtnqggpxng.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zdqjudy.top/gtcyrrkthv.html

[Q53] 按条件删除
来源：http://hz.yanxiufei.cn/gtlnqcpfks.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jiagoushi.top/gtdezlgvvp.html

[Q54] 清空表
来源：http://hz.xziqi.cn/gtwrkzkqpg.html

TRUNCATE TABLE logs;
来源：http://hz.316326.xyz/gtlzoxegxq.html

[Q55] 排名（并列占位）
来源：http://hz.daria6918.cn/gtztyqwtai.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hnxiangtu.top/gtoqdrkwcm.html

[Q56] 密集排名（并列不占位）
来源：http://hz.smart0.xyz/gtftxtruwz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.tianlin.xyz/gtlicjnzju.html

[Q57] 行号
来源：http://hz.0kj1m.cn/gtgywipwdc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yangfankeji.com/gtbjzbsegn.html

[Q58] 累计求和
来源：http://hz.gaohongyu789.top/gthrurjktq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.tianlin.xyz/gtbuynyocu.html

[Q59] 分组内累计
来源：http://hz.cheryme.top/gtadcyxken.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.dianchejie.cn/gtxtanzwez.html

[Q60] 取上一行 / 下一行
来源：http://hz.ehwqpu.com/gtbhfpxfrq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yuanzhike.top/gttbjeppwb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.sweek.top/gtotjgkyvq.html

[Q61] 移动平均
来源：http://hz.mhx1999.top/gtahdfhhfp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hammf.cn/gthqhmavyt.html

[Q62] 分组占比
来源：http://hz.andypj.xyz/gtrxsjwsur.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtbrwssaak.html

[Q63] 开启事务
来源：http://hz.hammf.cn/gtdqbutgub.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.kuanghao11.cn/gturjwxufq.html

[Q64] 提交事务
来源：http://hz.jinqigfzy.top/gtkuoyzmif.html

COMMIT;
来源：http://hz.hywenlv.cn/gtirdsrora.html

[Q65] 回滚事务
来源：http://hz.zhengqikj.top/gtphwtyyga.html

ROLLBACK;
来源：http://hz.quarkkingdee.top/gtqacpymrb.html

[Q66] 行锁查询
来源：http://hz.tian-w.cn/gtdfselvfv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj202588.top/gtctkldziy.html

[Q67] 设置隔离级别
来源：http://hz.xingfuxueyuan.xyz/gtvuornbks.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhijiandao.cn/gttojzfmiv.html

[Q68] 保存点
来源：http://hz.jqgfzy.top/gtemrtlpyn.html

SAVEPOINT sp1;
来源：http://hz.shangyingyoupin.top/gtdtbmcvro.html

ROLLBACK TO sp1;
来源：http://hz.shuidangran.top/gtgfjwkooz.html

[Q69] 查看执行计划
来源：http://hz.jlsjyb.cn/gttikwxwms.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.vqdsnc.cn/gtujkkfyza.html

[Q70] 更新统计信息
来源：http://hz.chenlongwang.top/gtrpuiypbv.html

ANALYZE TABLE users;
来源：http://hz.haohaochexian.top/gtgvgshsdv.html

[Q71] 查看建表语句
来源：http://hz.ydzc1.top/gtvmtgurxy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.dashuyun.cn/gtcyqemiit.html

[Q72] 查看索引
来源：http://hz.daria6918.cn/gtxlcbyegi.html

SHOW INDEX FROM users;
来源：http://hz.yj20258.top/gtgkwtjblg.html

[Q73] 查看表状态
来源：http://hz.jinghuilouyu.cn/gtygyzjmai.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ybcxt.top/gtplnrilkr.html

[Q74] 强制使用索引
来源：http://hz.iojbl.cn/gtwtuwixkd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.guowangkeji.top/gtmfdypqff.html

[Q75] 日期格式化
来源：http://hz.nwbrower.top/gtzvwpviot.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hnxiangtu.top/gtpierxwhd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yuxming.cn/gtfrctpsgu.html

[Q76] 按天统计
来源：http://hz.zhoulong.xyz/gtapzejbge.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jiagoushi.top/gtmmvboytv.html

[Q77] 时间加减
来源：http://hz.svipenyu.cn/gtydkhwwkz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.vqdsnc.cn/gtshlkzrym.html

[Q78] 当前时间
来源：http://hz.bjfxy.top/gtladjfrpm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xylfe.cn/gtsmjmdjww.html

[Q79] 字符串拼接
来源：http://hz.yvedp.cn/gtyilpvedd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.chenlongwang.top/gtokeegfrz.html

[Q80] 字符串截取
来源：http://hz.tanke756.top/gtkaisopdt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.0kj1m.cn/gtdbzgioym.html

[Q81] 字符串替换
来源：http://hz.pycfn.com/gtjbojcojv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnqzz.top/gtkbprmyby.html

[Q82] 字符长度与字节长度
来源：http://hz.jinghuilouyu.cn/gtybdcepwc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jqgfzy.top/gtrhafdebq.html

[Q83] 大小写转换
来源：http://hz.mhx1999.top/gtsystlckr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhoulong.xyz/gtmgpizaul.html

[Q84] 去除首尾空格
来源：http://hz.iojbl.cn/gtmphmyilw.html

SELECT TRIM(name) FROM users;
来源：http://hz.yuanzhike.top/gthnimebaz.html

[Q85] 数值取整
来源：http://hz.gzhubu.top/gtmkqbgcoj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.pengpengdd.cyou/gtorskyois.html

[Q86] 读取 JSON 字段
来源：http://hz.sufxvd.cn/gtwtdtotal.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yvedp.cn/gthusecpek.html

[Q87] JSON 字段做条件
来源：http://hz.jqgfzy.top/gtadkhujph.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xingfuxueyuan.xyz/gtwyulukcp.html

[Q88] 行转列（条件聚合）
来源：http://hz.tian-w.cn/gttfgnhyha.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ybcxt.top/gtfwessiyl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhaomingkeji.xyz/gtpwuwnqat.html

[Q89] 判断表是否存在
来源：http://hz.zhixingplan.top/gtrbsydyye.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhixingplan.top/gtdetklqdj.html

[Q90] 生成序号列
来源：http://hz.shzxlz.cn/gtlqnyurxl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.fengsongda.top/gtxxxcuxij.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtcxjoyjjl.html

R. Bash 专题
来源：http://hz.zhaomingkeji.xyz/gtknonxjhu.html

================================================================================
来源：http://hz.jianghu66.top/gtiwllvouz.html

[R01] shebang 与严格模式
来源：http://hz.kuanghao11.cn/gtfekavfod.html

#!/usr/bin/env bash
来源：http://hz.gzhubu.top/gtptmaqvqx.html

set -euo pipefail
来源：http://hz.dashuyun.cn/gtitiwzafc.html

[R02] 变量赋值与使用
来源：http://hz.bjfxy.top/gthztzlzkr.html

name="Tom"; echo "$name"
来源：http://hz.wangshuangyany.cn/gtxclquzaq.html

[R03] 只读变量
来源：http://hz.ybcxt.top/gthkxixulv.html

readonly PI=3.14
来源：http://hz.pengpengdd.cyou/gtyprsmfon.html

[R04] 位置参数
来源：http://hz.0kj1m.cn/gtexvfdkfx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.daxiang520.top/gtmfvbrfjf.html

[R05] 参数默认值
来源：http://hz.sysykeji.top/gtteoxnfyv.html

name="${1:-default}"
来源：http://hz.xuanzx.com/gtvympbzza.html

[R06] 判断命令是否存在
来源：http://hz.yj20258.top/gtcaguuvra.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xuanzx.com/gtzpaqnqbh.html

[R07] if 判断文件
来源：http://hz.shzxlz.cn/gthgckrwgj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hongshengwenyu.top/gtsfzlugep.html

[R08] 数值比较
来源：http://hz.zhijiandao.cn/gtpsidhgtz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shzxlz.cn/gthwoketdv.html

[R09] 字符串比较
来源：http://hz.birdmap.top/gtlzugdnat.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.feifeiyinyue.top/gtfwdluenb.html

[R10] 正则匹配
来源：http://hz.zhaomingkeji.xyz/gtqlkqombg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenzaomai.com/gtwkwqmeqh.html

[R11] case 多分支
来源：http://hz.haohaochexian.top/gttozoodsq.html

case "$1" in
来源：http://hz.zhaomingkeji.xyz/gtfmzyoobu.html

start) echo "启动" ;;
来源：http://hz.redwolf501.top/gtytwrpbay.html

stop)  echo "停止" ;;
来源：http://hz.chenjidiqi.icu/gttjsjvckl.html

*)     echo "未知命令" ;;
来源：http://hz.yj20258.top/gtzjeeiryc.html

esac
来源：http://hz.xuanzx.com/gtosicdclf.html

[R12] for 遍历文件
来源：http://hz.iojbl.cn/gtifpqcjff.html

for f in *.txt; do echo "$f"; done
来源：http://hz.redwolf501.top/gtypmylsdu.html

[R13] for 计数循环
来源：http://hz.wangdashe.top/gtslnoigvb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yueranfly.top/gtympbbthe.html

[R14] C 风格 for
来源：http://hz.52xcode.cn/gtgsqzevdl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cashguo.top/gtdeaebtqd.html

[R15] while 逐行读文件
来源：http://hz.havefunace.top/gtgdecqutt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zdqjudy.top/gtozbirzef.html

[R16] until 等待条件
来源：http://hz.ydzc1.top/gttgxxrssw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.dianchejie.cn/gtnaalkjth.html

[R17] 数组定义与取值
来源：http://hz.zhongyouzk.top/gtqilglkys.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yueranfly.top/gtwiozudcy.html

[R18] 遍历数组
来源：http://hz.jinyuanbaomall.cn/gtnoveufpp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.guannengcc.top/gtqemycwsq.html

[R19] 数组长度
来源：http://hz.jqgfzy.top/gtsewhpodw.html

echo "${#arr[@]}"
来源：http://hz.jinqigfzy.top/gtwmzhsxod.html

[R20] 关联数组（字典）
来源：http://hz.ybcxt.top/gtsxabjdvg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.bjfxy.top/gtlznitykz.html

[R21] 字符串长度
来源：http://hz.meibo888.top/gtlvroblnb.html

echo "${#s}"
来源：http://hz.haohaochexian.top/gtzvyevkdi.html

[R22] 截取子串
来源：http://hz.jqgfzy.top/gtrxbjuioi.html

echo "${s:0:5}"
来源：http://hz.52xcode.cn/gtywbutyzf.html

[R23] 字符串替换
来源：http://hz.zycfv.cn/gtcxwwhbiz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.snrcjt.cn/gthlbnnbqa.html

[R24] 大小写转换
来源：http://hz.cheryme.top/gtuvvfpgfq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jiagoushi.top/gtafbjdmpa.html

[R25] 去后缀 / 去前缀
来源：http://hz.dianchejie.cn/gtcqxtmncx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hongshengwenyu.top/gtjwbnylvf.html

[R26] 命令替换
来源：http://hz.tian-w.cn/gtdxzqucyn.html

now=$(date +%F); echo "$now"
来源：http://hz.hongshengwenyu.top/gtrphmwdiw.html

[R27] 算术展开
来源：http://hz.jqgfzy.top/gtyrdwimmz.html

echo $((1 + 2 * 3))
来源：http://hz.zhoulong.xyz/gtzdxqqged.html

[R28] 浮点运算
来源：http://hz.hfpthk.cn/gtfehjutmr.html

echo "scale=2; 10/3" | bc
来源：http://hz.hnxiangtu.top/gtoaiyrlna.html

[R29] 定义函数
来源：http://hz.cdnleiting.top/gtdxvcoprf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.fengsongda.top/gtvoazrzce.html

[R30] 函数返回状态码
来源：http://hz.nwbrower.top/gtgvxczjyx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.haohaochexian.top/gtojwpvdjs.html

[R31] 局部变量
来源：http://hz.gogol.net.cn/gtokcwccrz.html

f() { local x=1; echo "$x"; }
来源：http://hz.nanxuanxn.top/gthzcmbnkr.html

[R32] 参数个数校验
来源：http://hz.yongpay.top/gtyeefxolh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xuetiantiany.cn/gtbevepwdg.html

[R33] 捕获错误并提示行号
来源：http://hz.zycfv.cn/gtpwsjxjxh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.cqqwz.cn/gtstgeqvqv.html

[R34] 退出时清理
来源：http://hz.hfpthk.cn/gtaiedlavo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sufxvd.cn/gtaxywmysy.html

[R35] 后台执行并等待
来源：http://hz.hywenlv.cn/gtxhmsgftv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yangfankeji.com/gteyfztspy.html

[R36] 并发执行多个任务
来源：http://hz.dashuyun.cn/gtntcpreoy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hfpthk.cn/gtwsmbuejy.html

[R37] 把输出赋给变量
来源：http://hz.smart0.xyz/gtapoziqlk.html

files=$(ls -1)
来源：http://hz.birdmap.top/gteeqxktkg.html

[R38] 管道串联
来源：http://hz.shangyingyoupin.top/gtqzzqwmfx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hywenlv.cn/gtutlfijjg.html

[R39] 重定向标准输出与错误
来源：http://hz.hywenlv.cn/gtfizmsubs.html

cmd > out.log 2>&1
来源：http://hz.shanyushiyangkeji.top/gtsymvyemq.html

[R40] 追加写日志
来源：http://hz.fengsongda.top/gtsknoship.html

echo "log" >> out.log
来源：http://hz.jlsjyb.cn/gtzyukgofu.html

[R41] 丢弃输出
来源：http://hz.jiagoushi.top/gtitdcnkjt.html

cmd >/dev/null 2>&1
来源：http://hz.tanke756.top/gtobzqtsgh.html

[R42] 输入重定向
来源：http://hz.hongshengwenyu.top/gtsmctvbet.html

wc -l < a.txt
来源：http://hz.hnqzz.top/gtwnzgeafd.html

[R43] 按名字查找文件
来源：http://hz.xingfuxueyuan.xyz/gtgfvazuvo.html

find . -name "*.log" -type f
来源：http://hz.zhongyouzk.top/gtqxsdxhmg.html

[R44] 按修改时间查找
来源：http://hz.havefunace.top/gtqhheezip.html

find . -mtime -7 -type f
来源：http://hz.shangyingyoupin.top/gtbraqsfbj.html

[R45] 批量删除
来源：http://hz.xingfuxueyuan.xyz/gtwgprntbx.html

find . -name "*.tmp" -delete
来源：http://hz.zhaomingkeji.xyz/gtzdkgbppr.html

[R46] 递归替换文件内容
来源：http://hz.yongpay.top/gtswjmhxim.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hysaishi.cn/gtutedfxow.html

[R47] sed 单行替换
来源：http://hz.chenzaomai.com/gtshcjclwf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj20258888.top/gtdwnwowbu.html

[R48] awk 取指定列
来源：http://hz.xziqi.cn/gtbkxdaizt.html

awk '{print $1, $3}' a.txt
来源：http://hz.daxiang520.top/gtcxmywdao.html

[R49] awk 带条件
来源：http://hz.wangshuangyany.cn/gtdgirmkwt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yanxiufei.cn/gtlbfeboip.html

[R50] awk 求和
来源：http://hz.jinqigfzy.top/gtfwyutssg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.vqdsnc.cn/gtikbtetpo.html

[R51] 排序去重取前几
来源：http://hz.shuidangran.top/gtkftzlrpa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zdqjudy.top/gtpnfllegf.html

[R52] 统计行数
来源：http://hz.zhoulong.xyz/gtpwwycmqp.html

wc -l a.txt
来源：http://hz.wangshuangyany.cn/gtjidzsnbz.html

[R53] 查看文件头与实时尾
来源：http://hz.ppjwa.cn/gtdtzzzoad.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hysaishi.cn/gtupmxsbyz.html

[R54] 比较两个文件
来源：http://hz.chenjidiqi.icu/gtvukttdxd.html

diff a.txt b.txt
来源：http://hz.zhijiandao.cn/gtqstzuxrt.html

[R55] 压缩与解压
来源：http://hz.pengpengdd.cyou/gtntklonxb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhijiandao.cn/gtcckqmqnc.html

[R56] 远程拷贝
来源：http://hz.hongshengwenyu.top/gtttexnbbt.html

scp file user@host:/path/
来源：http://hz.zycfv.cn/gtxvphhvxf.html

[R57] 远程执行命令
来源：http://hz.hysaishi.cn/gtqifllmwe.html

ssh user@host 'uptime'
来源：http://hz.wangshuangyany.cn/gtpdlnzqna.html

[R58] 下载文件
来源：http://hz.zhijiandao.cn/gtdcowvnca.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yangfankeji.com/gtgbwiemwz.html

[R59] 发 POST JSON
来源：http://hz.chenjidiqi.icu/gtsaizmeds.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.52xcode.cn/gtlntteqjp.html

[R60] 只看 HTTP 状态码
来源：http://hz.wangshuangyany.cn/gtzmjlicbt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ybcxt.top/gtggamjrcv.html

[R61] 磁盘占用
来源：http://hz.hongshengwenyu.top/gtqnmsxwgu.html

df -h;  du -sh *
来源：http://hz.zhaomingkeji.xyz/gtpwleezmm.html

[R62] 找最占空间的文件
来源：http://hz.sxryk.cn/gtrcrnjdgj.html

du -ah . | sort -rh | head -10
来源：http://hz.jiagoushi.top/gttnhwxoqd.html

[R63] 内存与进程
来源：http://hz.iojbl.cn/gtfpofbvtm.html

free -h;  ps aux | grep nginx
来源：http://hz.gzhubu.top/gthkxshdqt.html

[R64] 结束进程
来源：http://hz.jianghu66.top/gtqkxujukj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenzaomai.com/gttadhawdt.html

[R65] 查看端口占用
来源：http://hz.zhaomingkeji.xyz/gtvueqjayy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.daria6918.cn/gthdymqdxm.html

[R66] 定时任务
来源：http://hz.hnxiangtu.top/gtduzewmzs.html

crontab -e;  crontab -l
来源：http://hz.yanxiufei.cn/gtsoyxvwym.html

[R67] 生成随机十六进制串
来源：http://hz.dashuyun.cn/gtbgjpxphi.html

openssl rand -hex 16
来源：http://hz.tianlin.xyz/gtkxtcwrnt.html

[R68] 计算文件校验值
来源：http://hz.nanxinkj.top/gtmchpzlql.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.52xcode.cn/gtcwcmhmdy.html

[R69] 生成随机密码
来源：http://hz.shangyingyoupin.top/gtyexeoxkr.html

head -c 16 /dev/urandom | base64
来源：http://hz.nwbrower.top/gtovuqmjyk.html

[R70] 时间戳与互转
来源：http://hz.xuanzx.com/gtlyunrrwg.html

date +%s;  date -d @1700000000
来源：http://hz.yonumen.top/gtgmexcjmw.html

[R71] 日期格式化
来源：http://hz.gogol.net.cn/gtnrbgtdsb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.quarkkingdee.top/gtgvyhghro.html

[R72] 等待端口就绪
来源：http://hz.jiagoushi.top/gtxtbxmnxu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinqigufen.top/gtlrlodczy.html

[R73] 分割大日志
来源：http://hz.chenzaomai.com/gtsqhyopkq.html

split -l 1000 big.log part_
来源：http://hz.yanxiufei.cn/gtjlpyjynz.html

[R74] 批量重命名
来源：http://hz.pycfn.com/gtvjvrfaps.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jiagoushi.top/gtfxecuuzf.html

[R75] 导出环境变量
来源：http://hz.hnqzz.top/gtxsidupbe.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nanxinkj.top/gtxgxdiepw.html

[R76] 使用临时文件
来源：http://hz.hysaishi.cn/gtwtsvuddc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gtjewhiciz.html

[R77] 读取用户输入
来源：http://hz.gaohongyu789.top/gtyimftdql.html


<!-- 参考信息 -->