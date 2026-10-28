代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.bjfxy.top/gtmorxsemx.html

[Q26] 计数
来源：http://hz.ivvv.top/gtmvjdalhf.html

SELECT COUNT(*) FROM users;
来源：http://hz.zdqjudy.top/gtdshnuqcp.html

[Q27] 条件计数
来源：http://hz.sysykeji.top/gtlknqqohk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ywan-chungtsiang.top/gtvdfleegw.html

[Q28] 求和与平均
来源：http://hz.jianghu66.top/gtkdyfdrsa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhiwuduotai.top/gtyygwkzwk.html

[Q29] 最大最小值
来源：http://hz.sysykeji.top/gtublaxpeh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jiagoushi.top/gtibnzthsy.html

[Q30] 分组统计
来源：http://hz.cashguo.top/gtqgneppxi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtzncshtse.html

[Q31] 分组后过滤
来源：http://hz.hnqzz.top/gtudberiib.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yuxming.cn/gtocojotjq.html

[Q32] 分组拼接字符串
来源：http://hz.haohaochexian.top/gtxqguguui.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtesinznxc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.wangdashe.top/gtybrfippx.html

[Q33] 多列分组
来源：http://hz.yueranfly.top/gtmgopgvne.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xuetiantiany.cn/gtxladlopo.html

[Q34] 每组取第一条
来源：http://hz.shangyingyoupin.top/gtswxenmel.html

SELECT * FROM (
来源：http://hz.vqdsnc.cn/gtialyssoi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ywan-chungtsiang.top/gtgwttrgbs.html

) t WHERE rn = 1;
来源：http://hz.sxryk.cn/gtdvvliygy.html

[Q35] 内连接
来源：http://hz.redwolf501.top/gtlrmwpdtx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuetiantiany.cn/gtukrjukzk.html

[Q36] 左连接
来源：http://hz.0kj1m.cn/gtwlrvzqli.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sysykeji.top/gtxjzdexrb.html

[Q37] 右连接
来源：http://hz.aizwys.cn/gtynnmznnh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.pengpengdd.cyou/gtbgeiywbs.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jlsjyb.cn/gtwkjhwakc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinqigfzy.top/gtwjxopubi.html

[Q39] 自连接（查上下级）
来源：http://hz.nanxuanxn.top/gthdqmblqh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jlsjyb.cn/gtyvlyveds.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hywenlv.cn/gtletlbbks.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shuidangran.top/gtrbiuuulm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jianghu66.top/gtdirsjcff.html

[Q41] 多表连接
来源：http://hz.zhiwuduotai.top/gtxfldmsvq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xuetiantiany.cn/gtqwdkdnrk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yongpay.top/gtnktizwbb.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.tanke756.top/gtzvxreqsm.html

[Q42] 连接条件附加过滤
来源：http://hz.ivvv.top/gtlfnwvrgs.html

SELECT u.name, o.amount FROM users u
来源：http://hz.wangdashe.top/gtreewkwvq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.fzhhl.top/gtzjfpyqym.html

[Q43] 标量子查询
来源：http://hz.nanxinkj.top/gtapurxjlz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sufxvd.cn/gtgiwbduve.html

[Q44] IN 子查询
来源：http://hz.shuidangran.top/gtcnnlntmn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jqgufenzy.top/gtxpvejibx.html

[Q45] EXISTS 判断存在
来源：http://hz.andypj.xyz/gtuiwqnzib.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigfzy.top/gtrvusynsy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.snrcjt.cn/gtznmiqvlv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cqqwz.cn/gtkyfaozjs.html

[Q47] 与平均值比较
来源：http://hz.316326.xyz/gtmmiyxlew.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shanyushiyangtech.top/gtkmpgkqbi.html

[Q48] CTE 公用表表达式
来源：http://hz.nwbrower.top/gtjtelfoty.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jiagoushi.top/gtqcnkpaet.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ydjk.org.cn/gtgvcsyukz.html

[Q49] 更新单行
来源：http://hz.pycfn.com/gtjdjcnpma.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hnqzz.top/gtatrmtwrv.html

[Q50] 批量更新
来源：http://hz.zhijiandao.cn/gtzhjuvrce.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hammf.cn/gtargcbfgr.html

[Q51] 用子查询更新
来源：http://hz.xuetiantiany.cn/gtjosfokcf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gzhubu.top/gtnzulgjjq.html

[Q52] 删除指定行
来源：http://hz.zhongyouzk.top/gtuzmqnxfn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.vqdsnc.cn/gtfztyjkfv.html

[Q53] 按条件删除
来源：http://hz.kuanghao11.cn/gtxbunwoih.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.svipenyu.cn/gtcjkvtabl.html

[Q54] 清空表
来源：http://hz.bjfxy.top/gtajcocosi.html

TRUNCATE TABLE logs;
来源：http://hz.shzxlz.cn/gtlcblumbz.html

[Q55] 排名（并列占位）
来源：http://hz.zdqjudy.top/gtxqpzfgru.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.haohaochexian.top/gteywqtuum.html

[Q56] 密集排名（并列不占位）
来源：http://hz.kuanghao11.cn/gtghmuhmcp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nanxuanxn.top/gtqfvfalvx.html

[Q57] 行号
来源：http://hz.xziqi.cn/gtavxkcrcp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yueranfly.top/gtjhhjeyno.html

[Q58] 累计求和
来源：http://hz.iojbl.cn/gtdfpgugha.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yueranfly.top/gtaqislznz.html

[Q59] 分组内累计
来源：http://hz.shanyushiyangtech.top/gtdahpxpjs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yanxiufei.cn/gthemnrdfv.html

[Q60] 取上一行 / 下一行
来源：http://hz.dashuyun.cn/gtqtzoehfd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hywenlv.cn/gtfqfwacuv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ehwqpu.com/gtfbucfvbr.html

[Q61] 移动平均
来源：http://hz.yuanzhike.top/gtsmolznzd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.fengsongda.top/gtarmjxyqk.html

[Q62] 分组占比
来源：http://hz.meibo888.top/gtkdgpkmfv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtixuqdoal.html

[Q63] 开启事务
来源：http://hz.nwbrower.top/gtztitwwwm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zdqjudy.top/gtzcdczpsk.html

[Q64] 提交事务
来源：http://hz.yuanzhike.top/gtlriomkoz.html

COMMIT;
来源：http://hz.jinqigfzy.top/gtxhifvwlm.html

[Q65] 回滚事务
来源：http://hz.chenlongwang.top/gtnlwckdju.html

ROLLBACK;
来源：http://hz.hywenlv.cn/gtiohhwnap.html

[Q66] 行锁查询
来源：http://hz.shanyushiyangtech.top/gtkugyrgqp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yanxiufei.cn/gtclvultpv.html

[Q67] 设置隔离级别
来源：http://hz.nwbrower.top/gtdgljqpjt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nanxinkj.top/gtfeixuyfc.html

[Q68] 保存点
来源：http://hz.havefunace.top/gtewrrotke.html

SAVEPOINT sp1;
来源：http://hz.aizwys.cn/gtmzpnquxm.html

ROLLBACK TO sp1;
来源：http://hz.guannengcc.top/gtpyrpfsqu.html

[Q69] 查看执行计划
来源：http://hz.bjfxy.top/gthjbccshs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.iojbl.cn/gtbmvikqdi.html

[Q70] 更新统计信息
来源：http://hz.sysykeji.top/gtkcdrrkti.html

ANALYZE TABLE users;
来源：http://hz.c1oappe.top/gtuylqyixx.html

[Q71] 查看建表语句
来源：http://hz.nanxinkj.top/gtanfsbznj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.guowangkeji.top/gtuuksihcv.html

[Q72] 查看索引
来源：http://hz.jyoumei.cn/gtpjhdfjfl.html

SHOW INDEX FROM users;
来源：http://hz.cashguo.top/gtoraluyto.html

[Q73] 查看表状态
来源：http://hz.jinqigufen.top/gtnuxxyixk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.svipenyu.cn/gtvkvglxzm.html

[Q74] 强制使用索引
来源：http://hz.dashuyun.cn/gtkputuezs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jqgufenzy.top/gtytdjsceb.html

[Q75] 日期格式化
来源：http://hz.cqqwz.cn/gtlhcfhyos.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.nwbrower.top/gtjbxoozje.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jyoumei.cn/gtqmnjimfc.html

[Q76] 按天统计
来源：http://hz.c1oappe.top/gtolmichsy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.kuanghao11.cn/gtaylvvfcd.html

[Q77] 时间加减
来源：http://hz.fzhhl.top/gtthlhnyvz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ybcxt.top/gtpdloykqh.html

[Q78] 当前时间
来源：http://hz.yuanzhike.top/gtelypdeqg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.kuanghao11.cn/gtkjlufuwg.html

[Q79] 字符串拼接
来源：http://hz.sufxvd.cn/gtpxkqpeqq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jyoumei.cn/gtvnprzmix.html

[Q80] 字符串截取
来源：http://hz.ydjk.org.cn/gtvrocwcbn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ivvv.top/gtuburdlli.html

[Q81] 字符串替换
来源：http://hz.feifeiyinyue.top/gtxgrevodg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydzc1.top/gtusiqkaaz.html

[Q82] 字符长度与字节长度
来源：http://hz.jqgfzy.top/gtojvnhlmg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtzsjrjxoe.html

[Q83] 大小写转换
来源：http://hz.nwbrower.top/gtxomemxss.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhixingplan.top/gtkoiescbx.html

[Q84] 去除首尾空格
来源：http://hz.iojbl.cn/gtaaqmvlzz.html

SELECT TRIM(name) FROM users;
来源：http://hz.snrcjt.cn/gtbkzjlvqs.html

[Q85] 数值取整
来源：http://hz.birdmap.top/gtglhtryib.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.daxiang520.top/gtzfdwnqgf.html

[Q86] 读取 JSON 字段
来源：http://hz.chenlongwang.top/gtzzdejkad.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhongyouzk.top/gtgxsncbyv.html

[Q87] JSON 字段做条件
来源：http://hz.ppjwa.cn/gttjxhjqfw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gzhubu.top/gtkknsqpky.html

[Q88] 行转列（条件聚合）
来源：http://hz.fengsongda.top/gtpauoperg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhiwuduotai.top/gtnuuzdjqt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shanyushiyangtech.top/gtwrdjfvir.html

[Q89] 判断表是否存在
来源：http://hz.jyoumei.cn/gtxqpfhzqf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.fzhhl.top/gtpazdrwko.html

[Q90] 生成序号列
来源：http://hz.xinyue.icu/gtrphbpkir.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hongshengwenyu.top/gtszxgbhsw.html

================================================================================
来源：http://hz.jiagoushi.top/gtdesjwtlq.html

R. Bash 专题
来源：http://hz.zhijiandao.cn/gtbikfmnqk.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtpvlsfjvv.html

[R01] shebang 与严格模式
来源：http://hz.yongpay.top/gtocujngpc.html

#!/usr/bin/env bash
来源：http://hz.vqdsnc.cn/gtsfqdvlzw.html

set -euo pipefail
来源：http://hz.ydzc1.top/gtpfeqcmjo.html

[R02] 变量赋值与使用
来源：http://hz.shanyushiyangkeji.top/gtddnzkjqe.html

name="Tom"; echo "$name"
来源：http://hz.zhiwuduotai.top/gtpbyzgeic.html

[R03] 只读变量
来源：http://hz.ydzc1.top/gtiphhrhzy.html

readonly PI=3.14
来源：http://hz.svipenyu.cn/gtvdwgesio.html

[R04] 位置参数
来源：http://hz.sysykeji.top/gtvqzshcft.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.wangshuangyany.cn/gtwezayxpf.html

[R05] 参数默认值
来源：http://hz.316326.xyz/gtgyizkttb.html

name="${1:-default}"
来源：http://hz.aibaodan.cn/gtyjjboaus.html

[R06] 判断命令是否存在
来源：http://hz.hnxiangtu.top/gtrhnhthon.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.bjfxy.top/gtvvjevoqf.html

[R07] if 判断文件
来源：http://hz.aibaodan.cn/gtkgutiofm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shanyushiyangtech.top/gtdpcllfau.html

[R08] 数值比较
来源：http://hz.jinqigufen.top/gtpuekytvk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xingfuxueyuan.xyz/gtqkomrten.html

[R09] 字符串比较
来源：http://hz.tanke756.top/gtgglskwlk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yangfankeji.com/gtvdrtnddi.html

[R10] 正则匹配
来源：http://hz.daxiang520.top/gtvolymhcu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.fengsongda.top/gtefkjjaii.html

[R11] case 多分支
来源：http://hz.yj20258.top/gtocykmsdz.html

case "$1" in
来源：http://hz.gzhubu.top/gtottxavjx.html

start) echo "启动" ;;
来源：http://hz.0kj1m.cn/gthvtkkivd.html

stop)  echo "停止" ;;
来源：http://hz.jiagoushi.top/gtgazjmser.html

*)     echo "未知命令" ;;
来源：http://hz.zycfv.cn/gtwzqwrlia.html

esac
来源：http://hz.kuanghao11.cn/gtueteycms.html

[R12] for 遍历文件
来源：http://hz.9152youxi.cn/gtdherrhcd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.havefunace.top/gteiecqktl.html

[R13] for 计数循环
来源：http://hz.jlsjyb.cn/gtcmbgeodk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.iojbl.cn/gtcbyzkpky.html

[R14] C 风格 for
来源：http://hz.ehwqpu.com/gtqpzpwdng.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jianghu66.top/gtzgghamee.html

[R15] while 逐行读文件
来源：http://hz.shanyushiyangtech.top/gtaokmbhcb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.fengsongda.top/gtvfqyfvjj.html

[R16] until 等待条件
来源：http://hz.jlsjyb.cn/gtnbxbylgp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtxyzkivwt.html

[R17] 数组定义与取值
来源：http://hz.tian-w.cn/gtqjywwgus.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.9152youxi.cn/gtzdqlgurt.html

[R18] 遍历数组
来源：http://hz.sxryk.cn/gtzskuclog.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jiagoushi.top/gtfvxbogtp.html

[R19] 数组长度
来源：http://hz.wangshuangyany.cn/gtxsfyfqca.html

echo "${#arr[@]}"
来源：http://hz.sufxvd.cn/gtrjwsyaxf.html

[R20] 关联数组（字典）
来源：http://hz.zhiwuduotai.top/gthuqlxsve.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangkeji.top/gtfaedxfew.html

[R21] 字符串长度
来源：http://hz.ehwqpu.com/gthkjdylwh.html

echo "${#s}"
来源：http://hz.fzhhl.top/gtzysqbamg.html

[R22] 截取子串
来源：http://hz.bjfxy.top/gtuoookyys.html

echo "${s:0:5}"
来源：http://hz.cucudq.cn/gtfwhyxoyq.html

[R23] 字符串替换
来源：http://hz.hywenlv.cn/gtsajqygtl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.quarkkingdee.top/gtwewmttup.html

[R24] 大小写转换
来源：http://hz.jinghuilouyu.cn/gtkvcastoe.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yangfankeji.com/gtaqfivhyf.html

[R25] 去后缀 / 去前缀
来源：http://hz.andypj.xyz/gtdtjesjgn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xinyue.icu/gtwiuvxsgv.html

[R26] 命令替换
来源：http://hz.nanxinkj.top/gtomdgddgd.html

now=$(date +%F); echo "$now"
来源：http://hz.cashguo.top/gtjndriucv.html

[R27] 算术展开
来源：http://hz.birdmap.top/gtiesnglhz.html

echo $((1 + 2 * 3))
来源：http://hz.nanxinkj.top/gtkmrgnusw.html

[R28] 浮点运算
来源：http://hz.tanke756.top/gtpxvgruld.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenlongwang.top/gtlyztcuin.html

[R29] 定义函数
来源：http://hz.ybcxt.top/gttwvmahyb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhongyouzk.top/gtxvfesyan.html

[R30] 函数返回状态码
来源：http://hz.yj20258.top/gttdbddktq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pengpengdd.cyou/gtlxzrpmuz.html

[R31] 局部变量
来源：http://hz.gogol.net.cn/gtusvhlskh.html

f() { local x=1; echo "$x"; }
来源：http://hz.yanxiufei.cn/gthcpwmxbe.html

[R32] 参数个数校验
来源：http://hz.zhoulong.xyz/gtinlwabty.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.chenlongwang.top/gtioqisndn.html

[R33] 捕获错误并提示行号
来源：http://hz.haohaochexian.top/gtikgkqdhv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.chenzaomai.com/gtsfbkwfdq.html

[R34] 退出时清理
来源：http://hz.zhaomingkeji.xyz/gtqikdegve.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cheryme.top/gtzzktoata.html

[R35] 后台执行并等待
来源：http://hz.hywenlv.cn/gtcwdecdry.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xziqi.cn/gtbqbzwpnv.html

[R36] 并发执行多个任务
来源：http://hz.yangfankeji.com/gtxdrkkszl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hywenlv.cn/gtgpwswynf.html

[R37] 把输出赋给变量
来源：http://hz.jianghu66.top/gtmumffxuc.html

files=$(ls -1)
来源：http://hz.jqgufenzy.top/gtwtraydnn.html

[R38] 管道串联
来源：http://hz.shuidangran.top/gtfryelkka.html

cat a.txt | grep -i error | wc -l
来源：http://hz.fzhhl.top/gtvgczoycp.html

[R39] 重定向标准输出与错误
来源：http://hz.dianchejie.cn/gtwmgijeji.html

cmd > out.log 2>&1
来源：http://hz.hywenlv.cn/gtjzdyohdh.html

[R40] 追加写日志
来源：http://hz.gaohongyu789.top/gtrlwxuvpg.html

echo "log" >> out.log
来源：http://hz.yuanzhike.top/gtcbaxtmzn.html

[R41] 丢弃输出
来源：http://hz.gaohongyu789.top/gtjzbjnqsx.html

cmd >/dev/null 2>&1
来源：http://hz.ywan-chungtsiang.top/gtzvqebmon.html

[R42] 输入重定向
来源：http://hz.vqdsnc.cn/gtashtokpe.html

wc -l < a.txt
来源：http://hz.fzhhl.top/gtuywlvjrm.html

[R43] 按名字查找文件
来源：http://hz.gaohongyu789.top/gtlkyzvffx.html

find . -name "*.log" -type f
来源：http://hz.fengsongda.top/gtcqybwvov.html

[R44] 按修改时间查找
来源：http://hz.yangfankeji.com/gtxgcqbkkf.html

find . -mtime -7 -type f
来源：http://hz.xingfuxueyuan.xyz/gtbyxcyhgb.html

[R45] 批量删除
来源：http://hz.cqqwz.cn/gtwxawalml.html

find . -name "*.tmp" -delete
来源：http://hz.aizwys.cn/gttadlxpjo.html

[R46] 递归替换文件内容
来源：http://hz.52xcode.cn/gthfjyfauv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.quarkkingdee.top/gtuerbsayc.html

[R47] sed 单行替换
来源：http://hz.zhixingplan.top/gtcyoqubtx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shuidangran.top/gtofkfaler.html

[R48] awk 取指定列
来源：http://hz.xinyue.icu/gtcuklnqmw.html

awk '{print $1, $3}' a.txt
来源：http://hz.zycfv.cn/gttwencqpu.html

[R49] awk 带条件
来源：http://hz.jianghu66.top/gtehyfyckt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhiwuduotai.top/gtevtqzklm.html

[R50] awk 求和
来源：http://hz.gaohongyu789.top/gtggfdvqnb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhongyouzk.top/gtscsityyk.html

[R51] 排序去重取前几
来源：http://hz.zhaomingkeji.xyz/gtnlvaglsl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yueranfly.top/gtesnifslo.html

[R52] 统计行数
来源：http://hz.zhaomingkeji.xyz/gtzignzojp.html

wc -l a.txt
来源：http://hz.gaohongyu789.top/gtmdjsgiaw.html

[R53] 查看文件头与实时尾
来源：http://hz.svipenyu.cn/gtpnaulixs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhiwuduotai.top/gtuvvhruvc.html

[R54] 比较两个文件
来源：http://hz.daxiang520.top/gthcuhgsuj.html

diff a.txt b.txt
来源：http://hz.zdqjudy.top/gtxriasyey.html

[R55] 压缩与解压
来源：http://hz.zhongyouzk.top/gtesiqfdfp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nwbrower.top/gtivmngsjf.html

[R56] 远程拷贝
来源：http://hz.zhiwuduotai.top/gtxfpkukbn.html

scp file user@host:/path/
来源：http://hz.hongshengwenyu.top/gtsszokole.html

[R57] 远程执行命令
来源：http://hz.nwbrower.top/gtzeplapdp.html

ssh user@host 'uptime'
来源：http://hz.ywan-chungtsiang.top/gtmmdrzgwl.html

[R58] 下载文件
来源：http://hz.sysykeji.top/gtwanotute.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zycfv.cn/gtrodgaplv.html

[R59] 发 POST JSON
来源：http://hz.svipenyu.cn/gtvhisnvof.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuanzhike.top/gtcqdzmqsb.html

[R60] 只看 HTTP 状态码
来源：http://hz.shuidangran.top/gteqvfhudm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zycfv.cn/gtayncahbp.html

[R61] 磁盘占用
来源：http://hz.cucudq.cn/gtjbwomjif.html

df -h;  du -sh *
来源：http://hz.zhiwuduotai.top/gtrrclhgws.html

[R62] 找最占空间的文件
来源：http://hz.yj202588.top/gtrtccwnun.html

du -ah . | sort -rh | head -10
来源：http://hz.xinyue.icu/gtcyktjiqk.html

[R63] 内存与进程
来源：http://hz.fengsongda.top/gtwjmeybhn.html

free -h;  ps aux | grep nginx
来源：http://hz.quarkkingdee.top/gtmoixxdhe.html

[R64] 结束进程
来源：http://hz.meibo888.top/gtwsnbyzox.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hfpthk.cn/gtepozmtlo.html

[R65] 查看端口占用
来源：http://hz.xinyue.icu/gtmwjvpwyt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.andypj.xyz/gtigxafywv.html

[R66] 定时任务
来源：http://hz.andypj.xyz/gtwivrbslo.html

crontab -e;  crontab -l
来源：http://hz.fengsongda.top/gtogghccxz.html

[R67] 生成随机十六进制串
来源：http://hz.pycfn.com/gtamiepvfa.html

openssl rand -hex 16
来源：http://hz.nwbrower.top/gtmdwkxpxc.html

[R68] 计算文件校验值
来源：http://hz.tian-w.cn/gtzyghleoy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.daxiang520.top/gtbbsbevqz.html

[R69] 生成随机密码
来源：http://hz.cqqwz.cn/gtreudfeup.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhoulong.xyz/gtlymhfuni.html

[R70] 时间戳与互转
来源：http://hz.hysaishi.cn/gtpnkthigp.html

date +%s;  date -d @1700000000
来源：http://hz.aizwys.cn/gtmvzhjzww.html

[R71] 日期格式化
来源：http://hz.yvedp.cn/gtccfgwrkh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xziqi.cn/gtieacnvkm.html

[R72] 等待端口就绪
来源：http://hz.shangyingyoupin.top/gtyfswuyah.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinqigufen.top/gtweoaxori.html

[R73] 分割大日志
来源：http://hz.zhijiandao.cn/gtbanqdlxh.html

split -l 1000 big.log part_
来源：http://hz.kuanghao11.cn/gtbhrxnlnm.html

[R74] 批量重命名
来源：http://hz.pengpengdd.cyou/gtforpscsw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tian-w.cn/gtbaepniiv.html

[R75] 导出环境变量
来源：http://hz.sxryk.cn/gtxpgogkvy.html


<!-- 参考信息 -->