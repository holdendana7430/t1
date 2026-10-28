代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.c1oappe.top/gtyyzswhmd.html

[Q26] 计数
来源：http://hz.quarkkingdee.top/gtjzxukkwa.html

SELECT COUNT(*) FROM users;
来源：http://hz.zycfv.cn/gtefcurpnc.html

[Q27] 条件计数
来源：http://hz.chenjidiqi.icu/gtpnzmfdlq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xinyue.icu/gtejcjvlio.html

[Q28] 求和与平均
来源：http://hz.aibaodan.cn/gtuatgaupj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.redwolf501.top/gtpcjewawx.html

[Q29] 最大最小值
来源：http://hz.xziqi.cn/gtgktkfhkw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.snrcjt.cn/gtpcfuljmm.html

[Q30] 分组统计
来源：http://hz.zhiwuduotai.top/gtzemuaagb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gtaqbrixmf.html

[Q31] 分组后过滤
来源：http://hz.ydjk.org.cn/gtidnzjtih.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.dianchejie.cn/gtzqfbwzgo.html

[Q32] 分组拼接字符串
来源：http://hz.haohaochexian.top/gtqcdqnmyd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtpdnnpmdo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cdnleiting.top/gttqmnfoxt.html

[Q33] 多列分组
来源：http://hz.0kj1m.cn/gtbzvwuzgc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hywenlv.cn/gtqyxegvhn.html

[Q34] 每组取第一条
来源：http://hz.shuidangran.top/gtnoqfbgqi.html

SELECT * FROM (
来源：http://hz.zhoulong.xyz/gtpyipiwcp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnqzz.top/gtnfowwqbe.html

) t WHERE rn = 1;
来源：http://hz.yj20258888.top/gtnsfqxbiq.html

[Q35] 内连接
来源：http://hz.yonumen.top/gtcylempmm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnxiangtu.top/gtgngmmyti.html

[Q36] 左连接
来源：http://hz.fengsongda.top/gtxilhljae.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tianlin.xyz/gthwnjilfe.html

[Q37] 右连接
来源：http://hz.zhongyouzk.top/gtesgfqola.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.daxiang520.top/gtkizxugrj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xingfuxueyuan.xyz/gtjmkafvkc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhijiandao.cn/gtsekzflgg.html

[Q39] 自连接（查上下级）
来源：http://hz.svipenyu.cn/gtcpwenvcv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ydjk.org.cn/gtyncuncsb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sxryk.cn/gtmbjyteuc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xziqi.cn/gtzqrbismu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenjidiqi.icu/gtvkfcuukw.html

[Q41] 多表连接
来源：http://hz.yj20258.top/gtjjeiyusl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hnqzz.top/gtlkbbwyzb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.aibaodan.cn/gtsnbxnceq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhijiandao.cn/gtuoofgrmg.html

[Q42] 连接条件附加过滤
来源：http://hz.sysykeji.top/gtbskvrlom.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ivvv.top/gthekwrjba.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sufxvd.cn/gtcebeeabj.html

[Q43] 标量子查询
来源：http://hz.gzhubu.top/gtxgqdnmpq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yongpay.top/gtgumpgmyl.html

[Q44] IN 子查询
来源：http://hz.hywenlv.cn/gtzibvmdvw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shzxlz.cn/gtdmlzflbd.html

[Q45] EXISTS 判断存在
来源：http://hz.shanyushiyangtech.top/gtzxyyeitk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.daria6918.cn/gtbadoarub.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shangyingyoupin.top/gtlvuoobvw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guowangkeji.top/gtcfhknjox.html

[Q47] 与平均值比较
来源：http://hz.yongpay.top/gttzfrbogp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.c1oappe.top/gtrremxsmx.html

[Q48] CTE 公用表表达式
来源：http://hz.ybcxt.top/gtjiernlan.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.wangdashe.top/gttwkqlmmj.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhijiandao.cn/gtmwjbynmq.html

[Q49] 更新单行
来源：http://hz.gaohongyu789.top/gtzuiqewgp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.tianlin.xyz/gtgxrpauuq.html

[Q50] 批量更新
来源：http://hz.dashuyun.cn/gtnoqxwswd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.kuanghao11.cn/gtpkzmqocy.html

[Q51] 用子查询更新
来源：http://hz.yangfankeji.com/gtnktywbpj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.kuanghao11.cn/gtvsyyhkgv.html

[Q52] 删除指定行
来源：http://hz.pengpengdd.cyou/gtsrutkvfj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cashguo.top/gtzifezvmx.html

[Q53] 按条件删除
来源：http://hz.wangshuangyany.cn/gtqbaszypf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ybcxt.top/gtuqyevvhn.html

[Q54] 清空表
来源：http://hz.aibaodan.cn/gtvfcdymur.html

TRUNCATE TABLE logs;
来源：http://hz.xuanzx.com/gtumacvfpm.html

[Q55] 排名（并列占位）
来源：http://hz.nwbrower.top/gtyvkpybrl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jqgufenzy.top/gtaojkpoby.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinyuanbaomall.cn/gtfnpwwkan.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.pycfn.com/gtbgcutjra.html

[Q57] 行号
来源：http://hz.zhengqikj.top/gtgxzbedqn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhijiandao.cn/gtualplyzq.html

[Q58] 累计求和
来源：http://hz.mhx1999.top/gtuniwnmgo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shzxlz.cn/gttwimyais.html

[Q59] 分组内累计
来源：http://hz.jinqigfzy.top/gtdkgezcwi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.wangdashe.top/gtzvvihdps.html

[Q60] 取上一行 / 下一行
来源：http://hz.birdmap.top/gtnhvxrnxr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.fengsongda.top/gtcrcgtvcf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yuxming.cn/gtznilwryo.html

[Q61] 移动平均
来源：http://hz.smart0.xyz/gtfqyqkhfh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yanxiufei.cn/gttahpiwhd.html

[Q62] 分组占比
来源：http://hz.hnqzz.top/gtujtittgb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gtlbnchyrb.html

[Q63] 开启事务
来源：http://hz.zhiwuduotai.top/gtamefrxxc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ybcxt.top/gtsdgixmma.html

[Q64] 提交事务
来源：http://hz.svipenyu.cn/gtbnbsyuxt.html

COMMIT;
来源：http://hz.pengpengdd.cyou/gtuozipzhw.html

[Q65] 回滚事务
来源：http://hz.jlsjyb.cn/gtxnfrifal.html

ROLLBACK;
来源：http://hz.birdmap.top/gtrtdwtuwt.html

[Q66] 行锁查询
来源：http://hz.guannengcc.top/gtxqkwbhwv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jqgfzy.top/gtaximnpnp.html

[Q67] 设置隔离级别
来源：http://hz.feifeiyinyue.top/gtgpgusdgf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hongshengwenyu.top/gtkitqieis.html

[Q68] 保存点
来源：http://hz.havefunace.top/gtncjppxfv.html

SAVEPOINT sp1;
来源：http://hz.chenlongwang.top/gtosxnmurg.html

ROLLBACK TO sp1;
来源：http://hz.hysaishi.cn/gtzdqiwjpq.html

[Q69] 查看执行计划
来源：http://hz.cheryme.top/gtxflisvdd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.fengsongda.top/gtwdablilz.html

[Q70] 更新统计信息
来源：http://hz.sweek.top/gtlumdmpsx.html

ANALYZE TABLE users;
来源：http://hz.9152youxi.cn/gtvssvdqhn.html

[Q71] 查看建表语句
来源：http://hz.cdnleiting.top/gttjaissli.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.guowangkeji.top/gtrxcthkrx.html

[Q72] 查看索引
来源：http://hz.52xcode.cn/gtgajompfa.html

SHOW INDEX FROM users;
来源：http://hz.316326.xyz/gtwmwrgawd.html

[Q73] 查看表状态
来源：http://hz.xylfe.cn/gtxkpxwirt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zdqjudy.top/gtspscdden.html

[Q74] 强制使用索引
来源：http://hz.dianchejie.cn/gtojezrjkw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.pycfn.com/gtjhryzhww.html

[Q75] 日期格式化
来源：http://hz.hammf.cn/gtfmbbhxcs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.vqdsnc.cn/gtehpckjkn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.dashuyun.cn/gtgjzrbmhr.html

[Q76] 按天统计
来源：http://hz.gzhubu.top/gtdpylmhdj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hammf.cn/gtyjsmqzux.html

[Q77] 时间加减
来源：http://hz.xziqi.cn/gtrzpmsbbe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yj20258888.top/gtdzxhcwvd.html

[Q78] 当前时间
来源：http://hz.c1oappe.top/gtpnslcxff.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.316326.xyz/gtbpggjrke.html

[Q79] 字符串拼接
来源：http://hz.sxryk.cn/gtngpivlpg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zdqjudy.top/gtuygelzoc.html

[Q80] 字符串截取
来源：http://hz.svipenyu.cn/gtftzytfbc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.c1oappe.top/gteguqclov.html

[Q81] 字符串替换
来源：http://hz.shzxlz.cn/gteiiucmle.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jiagoushi.top/gtfnbcombx.html

[Q82] 字符长度与字节长度
来源：http://hz.guowangkeji.top/gtlidzbdlq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zycfv.cn/gtghwxmveu.html

[Q83] 大小写转换
来源：http://hz.ppjwa.cn/gtjisyyhea.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hnxiangtu.top/gtdacroadj.html

[Q84] 去除首尾空格
来源：http://hz.xziqi.cn/gtbzpwmsyl.html

SELECT TRIM(name) FROM users;
来源：http://hz.smart0.xyz/gttqceqmnx.html

[Q85] 数值取整
来源：http://hz.yongpay.top/gtpwgakwnv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hywenlv.cn/gtqqtzpyvb.html

[Q86] 读取 JSON 字段
来源：http://hz.yvedp.cn/gtvsugcgnm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenjidiqi.icu/gtvvonpsfo.html

[Q87] JSON 字段做条件
来源：http://hz.jinyuanbaomall.cn/gtjpdromke.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.dianchejie.cn/gtmnwnykyl.html

[Q88] 行转列（条件聚合）
来源：http://hz.zdqjudy.top/gtqtcdxqgl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.meibo888.top/gtkmrvqxdl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.birdmap.top/gtditkkdji.html

[Q89] 判断表是否存在
来源：http://hz.meibo888.top/gtxrginujv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.wangshuangyany.cn/gtljahuaif.html

[Q90] 生成序号列
来源：http://hz.ehwqpu.com/gteunyjocm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.quarkkingdee.top/gthtmhvosw.html

================================================================================
来源：http://hz.hysaishi.cn/gtyyzvbmql.html

R. Bash 专题
来源：http://hz.bjfxy.top/gtjoupwguv.html

================================================================================
来源：http://hz.svipenyu.cn/gtkycxppxi.html

[R01] shebang 与严格模式
来源：http://hz.svipenyu.cn/gtisadksbh.html

#!/usr/bin/env bash
来源：http://hz.shanyushiyangtech.top/gtfpdstwkz.html

set -euo pipefail
来源：http://hz.smart0.xyz/gtuxamecfq.html

[R02] 变量赋值与使用
来源：http://hz.xylfe.cn/gtxtnoefhr.html

name="Tom"; echo "$name"
来源：http://hz.chenjidiqi.icu/gtlgqpqqqf.html

[R03] 只读变量
来源：http://hz.fzhhl.top/gtlwsicvvd.html

readonly PI=3.14
来源：http://hz.ydzc1.top/gteobdwgrk.html

[R04] 位置参数
来源：http://hz.andypj.xyz/gtiyssfgxy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.fzhhl.top/gtbfoufmio.html

[R05] 参数默认值
来源：http://hz.guannengcc.top/gtkacxxcqo.html

name="${1:-default}"
来源：http://hz.tianlin.xyz/gtnuemqqxm.html

[R06] 判断命令是否存在
来源：http://hz.zhengqikj.top/gtkbnboemd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jqgfzy.top/gtzhdaswjv.html

[R07] if 判断文件
来源：http://hz.yj202588.top/gtgebyzwze.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jiagoushi.top/gtfmhxwtwk.html

[R08] 数值比较
来源：http://hz.zdqjudy.top/gtlqchaqsu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cucudq.cn/gtiaedvwui.html

[R09] 字符串比较
来源：http://hz.tian-w.cn/gtntxskqbu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenzaomai.com/gtnoacrgrv.html

[R10] 正则匹配
来源：http://hz.yonumen.top/gtnpafnewp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cashguo.top/gtvusrpfoe.html

[R11] case 多分支
来源：http://hz.cashguo.top/gtnndyastc.html

case "$1" in
来源：http://hz.jyoumei.cn/gtltzjynjn.html

start) echo "启动" ;;
来源：http://hz.hammf.cn/gtbmaalmtg.html

stop)  echo "停止" ;;
来源：http://hz.zhoulong.xyz/gtlrravvvj.html

*)     echo "未知命令" ;;
来源：http://hz.yueranfly.top/gtzqvaewvs.html

esac
来源：http://hz.vqdsnc.cn/gtghzmkxfv.html

[R12] for 遍历文件
来源：http://hz.zhoulong.xyz/gtlariecar.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj20258.top/gtwqoumucs.html

[R13] for 计数循环
来源：http://hz.cashguo.top/gtmxyesizx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yonumen.top/gtlpgsolfz.html

[R14] C 风格 for
来源：http://hz.yongpay.top/gtglfvqmtd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.mhx1999.top/gtiaojswap.html

[R15] while 逐行读文件
来源：http://hz.hnxiangtu.top/gtpkfsfbtc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sysykeji.top/gtrpskdxzu.html

[R16] until 等待条件
来源：http://hz.ehwqpu.com/gtrfcrdyfw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ehwqpu.com/gtmiotavdi.html

[R17] 数组定义与取值
来源：http://hz.xinyue.icu/gtvllhjwhv.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sweek.top/gtjffftogf.html

[R18] 遍历数组
来源：http://hz.shangyingyoupin.top/gtkdnhnrne.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ydzc1.top/gtabcjmuhi.html

[R19] 数组长度
来源：http://hz.tanke756.top/gtpmktwgjj.html

echo "${#arr[@]}"
来源：http://hz.nanxinkj.top/gtxhpudxuh.html

[R20] 关联数组（字典）
来源：http://hz.jinqigufen.top/gtftizwvjp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ybcxt.top/gttwbnphvy.html

[R21] 字符串长度
来源：http://hz.ppjwa.cn/gtbqgttckb.html

echo "${#s}"
来源：http://hz.birdmap.top/gtpapvbctc.html

[R22] 截取子串
来源：http://hz.zhongyouzk.top/gtpsitsaqk.html

echo "${s:0:5}"
来源：http://hz.pengpengdd.cyou/gtfsacivzo.html

[R23] 字符串替换
来源：http://hz.yuanzhike.top/gtniqmcily.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.feifeiyinyue.top/gtvctpdimd.html

[R24] 大小写转换
来源：http://hz.nanxuanxn.top/gtkirkzysu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhiwuduotai.top/gtwvvpntxt.html

[R25] 去后缀 / 去前缀
来源：http://hz.fengsongda.top/gtqabcjnaq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhijiandao.cn/gtbxvoopjl.html

[R26] 命令替换
来源：http://hz.cqqwz.cn/gtdzqaosce.html

now=$(date +%F); echo "$now"
来源：http://hz.ehwqpu.com/gtjzqkzmzl.html

[R27] 算术展开
来源：http://hz.cashguo.top/gtmtdlwxtc.html

echo $((1 + 2 * 3))
来源：http://hz.svipenyu.cn/gtysofmrtr.html

[R28] 浮点运算
来源：http://hz.xinyue.icu/gtcokgvgnl.html

echo "scale=2; 10/3" | bc
来源：http://hz.shuidangran.top/gtyjnfzawo.html

[R29] 定义函数
来源：http://hz.chenlongwang.top/gtwvtrfswu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cdnleiting.top/gtitxvfghi.html

[R30] 函数返回状态码
来源：http://hz.yueranfly.top/gtbdkfvdhm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hysaishi.cn/gtpdgzuhku.html

[R31] 局部变量
来源：http://hz.jinghuilouyu.cn/gttvnvjdhr.html

f() { local x=1; echo "$x"; }
来源：http://hz.nanxuanxn.top/gteriarkiw.html

[R32] 参数个数校验
来源：http://hz.jiagoushi.top/gtdsmvrjbt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.aizwys.cn/gtebijucod.html

[R33] 捕获错误并提示行号
来源：http://hz.ybcxt.top/gtcsddrted.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xinyue.icu/gtggnitkvm.html

[R34] 退出时清理
来源：http://hz.bjfxy.top/gtkdnttcyr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hammf.cn/gtbewlqwfd.html

[R35] 后台执行并等待
来源：http://hz.hammf.cn/gtagwtxlxd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.birdmap.top/gtzwyudqkg.html

[R36] 并发执行多个任务
来源：http://hz.0kj1m.cn/gtpdzqzqrp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zycfv.cn/gtwjuudcti.html

[R37] 把输出赋给变量
来源：http://hz.nanxinkj.top/gtrdzyjvvh.html

files=$(ls -1)
来源：http://hz.yuxming.cn/gtgrcllguf.html

[R38] 管道串联
来源：http://hz.sweek.top/gtrhwieoai.html

cat a.txt | grep -i error | wc -l
来源：http://hz.0kj1m.cn/gtyhfofqqm.html

[R39] 重定向标准输出与错误
来源：http://hz.pengpengdd.cyou/gtnzahlmiy.html

cmd > out.log 2>&1
来源：http://hz.jianghu66.top/gtwibkswpn.html

[R40] 追加写日志
来源：http://hz.chenjidiqi.icu/gthsjcnwzl.html

echo "log" >> out.log
来源：http://hz.gogol.net.cn/gtqepjbdma.html

[R41] 丢弃输出
来源：http://hz.smart0.xyz/gtcwhoccsx.html

cmd >/dev/null 2>&1
来源：http://hz.jianghu66.top/gtprlcyagi.html

[R42] 输入重定向
来源：http://hz.ydzc1.top/gtofdhnzjo.html

wc -l < a.txt
来源：http://hz.iojbl.cn/gtihmbneky.html

[R43] 按名字查找文件
来源：http://hz.jqgfzy.top/gtbhhfdarx.html

find . -name "*.log" -type f
来源：http://hz.xziqi.cn/gtciuzqiwq.html

[R44] 按修改时间查找
来源：http://hz.0kj1m.cn/gtfkasikpg.html

find . -mtime -7 -type f
来源：http://hz.ywan-chungtsiang.top/gtvytfqmex.html

[R45] 批量删除
来源：http://hz.zdqjudy.top/gtjbljwlck.html

find . -name "*.tmp" -delete
来源：http://hz.jinghuilouyu.cn/gtscduhrsh.html

[R46] 递归替换文件内容
来源：http://hz.feifeiyinyue.top/gtqxbemahr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shuidangran.top/gteitjygad.html

[R47] sed 单行替换
来源：http://hz.nwbrower.top/gtewhvewcm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xylfe.cn/gtciuzpwrz.html

[R48] awk 取指定列
来源：http://hz.sufxvd.cn/gtiutaqgap.html

awk '{print $1, $3}' a.txt
来源：http://hz.zycfv.cn/gtkvfkemrl.html

[R49] awk 带条件
来源：http://hz.hnqzz.top/gtmrdxkdgm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.sufxvd.cn/gtxpyghjxl.html

[R50] awk 求和
来源：http://hz.shanyushiyangkeji.top/gtycgcvgkv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gzhubu.top/gtubgkxfwr.html

[R51] 排序去重取前几
来源：http://hz.chenlongwang.top/gtdwgqoqty.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj20258888.top/gtzdnutcew.html

[R52] 统计行数
来源：http://hz.hammf.cn/gtydjcwjgg.html

wc -l a.txt
来源：http://hz.zycfv.cn/gtqcffkuya.html

[R53] 查看文件头与实时尾
来源：http://hz.wangdashe.top/gtjjxdihyw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.nanxuanxn.top/gtivdahjvf.html

[R54] 比较两个文件
来源：http://hz.shzxlz.cn/gtczhuelsg.html

diff a.txt b.txt
来源：http://hz.yangfankeji.com/gtwtilffsp.html

[R55] 压缩与解压
来源：http://hz.zhaomingkeji.xyz/gtyvmidrpy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tianlin.xyz/gtklxtwmyd.html

[R56] 远程拷贝
来源：http://hz.hnxiangtu.top/gtmqckqthk.html

scp file user@host:/path/
来源：http://hz.jyoumei.cn/gtfyitzffi.html

[R57] 远程执行命令
来源：http://hz.cashguo.top/gtvqiqzywa.html

ssh user@host 'uptime'
来源：http://hz.cqqwz.cn/gtthrlfcjq.html

[R58] 下载文件
来源：http://hz.zhijiandao.cn/gtxzbvikhi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj20258.top/gttjjtwjpw.html

[R59] 发 POST JSON
来源：http://hz.sysykeji.top/gtliglyehq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sweek.top/gttlepeumg.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenlongwang.top/gttfcogpjy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.chenjidiqi.icu/gtzuleiwjd.html

[R61] 磁盘占用
来源：http://hz.yj202588.top/gtnhbpcegg.html

df -h;  du -sh *
来源：http://hz.nwbrower.top/gtfpvblbel.html

[R62] 找最占空间的文件
来源：http://hz.ydjk.org.cn/gtidouiqho.html

du -ah . | sort -rh | head -10
来源：http://hz.tianlin.xyz/gtiehgukdd.html

[R63] 内存与进程
来源：http://hz.havefunace.top/gtdrwbqcmw.html

free -h;  ps aux | grep nginx
来源：http://hz.zhijiandao.cn/gtehpahcya.html

[R64] 结束进程
来源：http://hz.gotoacloud.top/gttxxtstfk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.vqdsnc.cn/gtmjfjovht.html

[R65] 查看端口占用
来源：http://hz.gotoacloud.top/gtdrkwyaok.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gotoacloud.top/gtwvcrcgda.html

[R66] 定时任务
来源：http://hz.nwbrower.top/gtbbslkzsf.html

crontab -e;  crontab -l
来源：http://hz.gzhubu.top/gtrgxeulpa.html

[R67] 生成随机十六进制串
来源：http://hz.xingfuxueyuan.xyz/gtxvncciyv.html

openssl rand -hex 16
来源：http://hz.cucudq.cn/gtsbtmywit.html

[R68] 计算文件校验值
来源：http://hz.zdqjudy.top/gtqvedcqge.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jyoumei.cn/gtsetlgowt.html

[R69] 生成随机密码
来源：http://hz.yuanzhike.top/gthsjvdcio.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinqigufen.top/gtlmrrgszc.html

[R70] 时间戳与互转
来源：http://hz.jinyuanbaomall.cn/gtqjldcysy.html

date +%s;  date -d @1700000000
来源：http://hz.yuxming.cn/gtivqttivf.html

[R71] 日期格式化
来源：http://hz.aizwys.cn/gturmxjybm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cucudq.cn/gtpqmwyywx.html

[R72] 等待端口就绪
来源：http://hz.tian-w.cn/gtwjkuigvk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.guannengcc.top/gtdmrsserj.html

[R73] 分割大日志
来源：http://hz.gzhubu.top/gtbjiwrfuf.html

split -l 1000 big.log part_
来源：http://hz.xylfe.cn/gthdusaygx.html

[R74] 批量重命名
来源：http://hz.bjfxy.top/gtkipwjfsu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.c1oappe.top/gtiiggjlls.html

[R75] 导出环境变量
来源：http://hz.jqgfzy.top/gtyqelvgpi.html


<!-- 参考信息 -->