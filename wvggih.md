代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cqqwz.cn/gtggfhdvkg.html

[Q26] 计数
来源：http://hz.ydjk.org.cn/gtipcucxgp.html

SELECT COUNT(*) FROM users;
来源：http://hz.quarkkingdee.top/gtpfbxnvhx.html

[Q27] 条件计数
来源：http://hz.ybcxt.top/gtcelfemtm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jyoumei.cn/gtykjcxgau.html

[Q28] 求和与平均
来源：http://hz.ydzc1.top/gtayismvcr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.svipenyu.cn/gtjmiivmml.html

[Q29] 最大最小值
来源：http://hz.hongshengwenyu.top/gtfkizwsfz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hongshengwenyu.top/gtbtvgdpgq.html

[Q30] 分组统计
来源：http://hz.bjfxy.top/gtycurjbbk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cqqwz.cn/gtqqbruorl.html

[Q31] 分组后过滤
来源：http://hz.ywan-chungtsiang.top/gtcacytlot.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hnxiangtu.top/gtsblgzlzj.html

[Q32] 分组拼接字符串
来源：http://hz.nanxuanxn.top/gttpjncazy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtazvovnuh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yuxming.cn/gtmctmrhaw.html

[Q33] 多列分组
来源：http://hz.yongpay.top/gthzvpnxjh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hongshengwenyu.top/gtpkvhgbvz.html

[Q34] 每组取第一条
来源：http://hz.mhx1999.top/gtomhpwzqy.html

SELECT * FROM (
来源：http://hz.sxryk.cn/gtlgyrcjdw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zycfv.cn/gtktqobchv.html

) t WHERE rn = 1;
来源：http://hz.guowangkeji.top/gtumasggyf.html

[Q35] 内连接
来源：http://hz.fzhhl.top/gtnvgmsexf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.dianchejie.cn/gtclrirtlf.html

[Q36] 左连接
来源：http://hz.fengsongda.top/gtpaxmcevj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ywan-chungtsiang.top/gtqaacewqq.html

[Q37] 右连接
来源：http://hz.quarkkingdee.top/gtbbfyjpmq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinghuilouyu.cn/gtixcoycxm.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ydjk.org.cn/gtomhbaoyx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.nanxuanxn.top/gtahvetnvk.html

[Q39] 自连接（查上下级）
来源：http://hz.zhaomingkeji.xyz/gtbvtsnsku.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.iojbl.cn/gtzwfasesb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yonumen.top/gtmwlvgcth.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cashguo.top/gtckjgkegd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.birdmap.top/gtfdubbisk.html

[Q41] 多表连接
来源：http://hz.chenjidiqi.icu/gtqdoytufn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.feifeiyinyue.top/gtvaxxsvxw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.tian-w.cn/gtrkvaheym.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.c1oappe.top/gtkdyskifg.html

[Q42] 连接条件附加过滤
来源：http://hz.fengsongda.top/gtpcbqjxpv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.kuanghao11.cn/gtfqpccqki.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nwbrower.top/gtdhpdstuj.html

[Q43] 标量子查询
来源：http://hz.zhiwuduotai.top/gtmgvwerux.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhoulong.xyz/gtgdqhjder.html

[Q44] IN 子查询
来源：http://hz.ppjwa.cn/gtdimjerha.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ehwqpu.com/gthywcmadl.html

[Q45] EXISTS 判断存在
来源：http://hz.gaohongyu789.top/gtycommllw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxuanxn.top/gtuiwrvkxx.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nanxinkj.top/gtfaqodxru.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.havefunace.top/gtlxxwsxjs.html

[Q47] 与平均值比较
来源：http://hz.quarkkingdee.top/gtolvkcbqo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.kuanghao11.cn/gtlhffyudp.html

[Q48] CTE 公用表表达式
来源：http://hz.shanyushiyangtech.top/gtquklhier.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.dianchejie.cn/gtcyozxsed.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jiagoushi.top/gthrexliqe.html

[Q49] 更新单行
来源：http://hz.zhoulong.xyz/gtoqeprohx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.tanke756.top/gtqkspffkd.html

[Q50] 批量更新
来源：http://hz.yvedp.cn/gtzsngxsbr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shzxlz.cn/gtvmgutwnj.html

[Q51] 用子查询更新
来源：http://hz.yvedp.cn/gtmxqlgkms.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yuxming.cn/gttjvykwvn.html

[Q52] 删除指定行
来源：http://hz.nwbrower.top/gtjqweryyh.html

DELETE FROM users WHERE id = 10;
来源：http://hz.mhx1999.top/gtrtdjemax.html

[Q53] 按条件删除
来源：http://hz.xylfe.cn/gtxzfoaflj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yongpay.top/gtnqtdhmvr.html

[Q54] 清空表
来源：http://hz.daria6918.cn/gtahhixisp.html

TRUNCATE TABLE logs;
来源：http://hz.nwbrower.top/gtubarukhk.html

[Q55] 排名（并列占位）
来源：http://hz.0kj1m.cn/gthcewjvay.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.aibaodan.cn/gtqhgsdzuu.html

[Q56] 密集排名（并列不占位）
来源：http://hz.52xcode.cn/gtwqwqytli.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yanxiufei.cn/gtoflxpvbw.html

[Q57] 行号
来源：http://hz.havefunace.top/gtzxzejgob.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gzhubu.top/gtlkghygqb.html

[Q58] 累计求和
来源：http://hz.pycfn.com/gtksebxipa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hywenlv.cn/gtuczmvxlv.html

[Q59] 分组内累计
来源：http://hz.kuanghao11.cn/gtbrqwkxsd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangtech.top/gtkmxffics.html

[Q60] 取上一行 / 下一行
来源：http://hz.andypj.xyz/gtlqwytolf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.daxiang520.top/gtrkwjnqgd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.smart0.xyz/gtxqhgytim.html

[Q61] 移动平均
来源：http://hz.xingfuxueyuan.xyz/gtqxbsknjg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtsrpdbwec.html

[Q62] 分组占比
来源：http://hz.mhx1999.top/gtqwfmgllm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.52xcode.cn/gtahhmqgwp.html

[Q63] 开启事务
来源：http://hz.shuidangran.top/gtazaviume.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ydjk.org.cn/gtedrxfvws.html

[Q64] 提交事务
来源：http://hz.xziqi.cn/gthjquscpb.html

COMMIT;
来源：http://hz.jinghuilouyu.cn/gtytuespeb.html

[Q65] 回滚事务
来源：http://hz.guowangkeji.top/gtipvlkaov.html

ROLLBACK;
来源：http://hz.cdnleiting.top/gtzduoqepq.html

[Q66] 行锁查询
来源：http://hz.yangfankeji.com/gtyzivkkra.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhaomingkeji.xyz/gtdhfyztns.html

[Q67] 设置隔离级别
来源：http://hz.zhiwuduotai.top/gtvfdeynaf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.sysykeji.top/gtockolqis.html

[Q68] 保存点
来源：http://hz.316326.xyz/gtoagfmyku.html

SAVEPOINT sp1;
来源：http://hz.jqgufenzy.top/gtgaektgkr.html

ROLLBACK TO sp1;
来源：http://hz.quarkkingdee.top/gtboujswwf.html

[Q69] 查看执行计划
来源：http://hz.yangfankeji.com/gtjlesphwd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ppjwa.cn/gtrhgmviqf.html

[Q70] 更新统计信息
来源：http://hz.haohaochexian.top/gtwiildilt.html

ANALYZE TABLE users;
来源：http://hz.jqgfzy.top/gtxegdtwae.html

[Q71] 查看建表语句
来源：http://hz.haohaochexian.top/gthufwldrg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cashguo.top/gtolqeqadm.html

[Q72] 查看索引
来源：http://hz.jqgufenzy.top/gtatxqmuoo.html

SHOW INDEX FROM users;
来源：http://hz.ywan-chungtsiang.top/gtxhephnnj.html

[Q73] 查看表状态
来源：http://hz.ehwqpu.com/gteordqrmi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.tanke756.top/gtyqmbgziv.html

[Q74] 强制使用索引
来源：http://hz.fengsongda.top/gtqbhzziew.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xuanzx.com/gtfuktjxih.html

[Q75] 日期格式化
来源：http://hz.9152youxi.cn/gtdaesblag.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.nanxuanxn.top/gtjqlicnng.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ywan-chungtsiang.top/gtfbngakka.html

[Q76] 按天统计
来源：http://hz.hnqzz.top/gtjaacwzek.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jyoumei.cn/gtnahnnmao.html

[Q77] 时间加减
来源：http://hz.sysykeji.top/gtmetudmxh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jqgufenzy.top/gtswkatfkb.html

[Q78] 当前时间
来源：http://hz.yongpay.top/gtfalveemg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.svipenyu.cn/gtsqdxtoli.html

[Q79] 字符串拼接
来源：http://hz.havefunace.top/gtpgzqlfmd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shanyushiyangkeji.top/gtupnrxgpp.html

[Q80] 字符串截取
来源：http://hz.ywan-chungtsiang.top/gtighzadvc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hywenlv.cn/gttxtrbfbw.html

[Q81] 字符串替换
来源：http://hz.jqgufenzy.top/gtlygarxiw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.meibo888.top/gtfsyikmgy.html

[Q82] 字符长度与字节长度
来源：http://hz.yj20258.top/gtwdzzzsrb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jqgfzy.top/gtprzpvjqw.html

[Q83] 大小写转换
来源：http://hz.nwbrower.top/gtngmzywet.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hnxiangtu.top/gtnfrabhcx.html

[Q84] 去除首尾空格
来源：http://hz.9152youxi.cn/gtmtthhbwy.html

SELECT TRIM(name) FROM users;
来源：http://hz.dianchejie.cn/gtvpmupgdk.html

[Q85] 数值取整
来源：http://hz.quarkkingdee.top/gteblupagn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhiwuduotai.top/gtvwvfnacr.html

[Q86] 读取 JSON 字段
来源：http://hz.wangshuangyany.cn/gtvgctlcqg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gzhubu.top/gtbnjgvbjh.html

[Q87] JSON 字段做条件
来源：http://hz.guannengcc.top/gtsnaiargq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.c1oappe.top/gtomsyomrn.html

[Q88] 行转列（条件聚合）
来源：http://hz.0kj1m.cn/gtvfxhljal.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.dashuyun.cn/gtgmzxgqty.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yanxiufei.cn/gtqzqnoyfj.html

[Q89] 判断表是否存在
来源：http://hz.cucudq.cn/gtzhxkhvhy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhiwuduotai.top/gtdcheruec.html

[Q90] 生成序号列
来源：http://hz.dashuyun.cn/gttwbyvrjg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hnqzz.top/gtltdffaem.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtyjtaeblw.html

R. Bash 专题
来源：http://hz.316326.xyz/gtcbkjnrfv.html

================================================================================
来源：http://hz.shuidangran.top/gtoblnkpiq.html

[R01] shebang 与严格模式
来源：http://hz.aibaodan.cn/gtnfpmlgua.html

#!/usr/bin/env bash
来源：http://hz.zdqjudy.top/gtrtjusoxm.html

set -euo pipefail
来源：http://hz.redwolf501.top/gtqiiitzlp.html

[R02] 变量赋值与使用
来源：http://hz.svipenyu.cn/gtnvwjzsge.html

name="Tom"; echo "$name"
来源：http://hz.cashguo.top/gtcwymmehj.html

[R03] 只读变量
来源：http://hz.daria6918.cn/gtzznhezra.html

readonly PI=3.14
来源：http://hz.pengpengdd.cyou/gtpwbozppi.html

[R04] 位置参数
来源：http://hz.ivvv.top/gtgiujouwp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.c1oappe.top/gtaimsilwv.html

[R05] 参数默认值
来源：http://hz.hongshengwenyu.top/gtsqtolfvt.html

name="${1:-default}"
来源：http://hz.tanke756.top/gtiizhveto.html

[R06] 判断命令是否存在
来源：http://hz.tanke756.top/gtszojgkhx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.52xcode.cn/gtwoltkfbk.html

[R07] if 判断文件
来源：http://hz.cashguo.top/gtugekblqu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.aibaodan.cn/gtvxswvebk.html

[R08] 数值比较
来源：http://hz.yongpay.top/gtkfqzysns.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.guowangkeji.top/gtwxgsqgzb.html

[R09] 字符串比较
来源：http://hz.fengsongda.top/gtqfbskoxs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ywan-chungtsiang.top/gtmweovzqk.html

[R10] 正则匹配
来源：http://hz.haohaochexian.top/gteonalplo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.0kj1m.cn/gtqvjeheya.html

[R11] case 多分支
来源：http://hz.jqgufenzy.top/gtitfbwpnh.html

case "$1" in
来源：http://hz.yueranfly.top/gtlhlwlgtf.html

start) echo "启动" ;;
来源：http://hz.zhaomingkeji.xyz/gtytzohoao.html

stop)  echo "停止" ;;
来源：http://hz.sweek.top/gtoyomzffa.html

*)     echo "未知命令" ;;
来源：http://hz.daria6918.cn/gtsuwgfeuu.html

esac
来源：http://hz.feifeiyinyue.top/gtxwkkkmpb.html

[R12] for 遍历文件
来源：http://hz.jinghuilouyu.cn/gtvtpjpxkv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.redwolf501.top/gtvnwnnnqu.html

[R13] for 计数循环
来源：http://hz.hywenlv.cn/gtxfneygib.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenlongwang.top/gthdzfgbid.html

[R14] C 风格 for
来源：http://hz.zycfv.cn/gteasfklnz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jlsjyb.cn/gtafoxktgo.html

[R15] while 逐行读文件
来源：http://hz.iojbl.cn/gtrqlnwpvb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.chenlongwang.top/gtwxdukbkg.html

[R16] until 等待条件
来源：http://hz.gaohongyu789.top/gtqusohhuz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ywan-chungtsiang.top/gtnljtzozy.html

[R17] 数组定义与取值
来源：http://hz.andypj.xyz/gtzkkaxjxg.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.meibo888.top/gtzrblosog.html

[R18] 遍历数组
来源：http://hz.sweek.top/gthuotddfo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhoulong.xyz/gtpbcesatt.html

[R19] 数组长度
来源：http://hz.jyoumei.cn/gtoxuggasd.html

echo "${#arr[@]}"
来源：http://hz.bjfxy.top/gtuzkhezcz.html

[R20] 关联数组（字典）
来源：http://hz.xziqi.cn/gtvufwdlic.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cdnleiting.top/gtdkylmcic.html

[R21] 字符串长度
来源：http://hz.yuanzhike.top/gtwlhbwvsv.html

echo "${#s}"
来源：http://hz.sweek.top/gtubkjzkyv.html

[R22] 截取子串
来源：http://hz.ivvv.top/gtwulvvijl.html

echo "${s:0:5}"
来源：http://hz.yangfankeji.com/gtxyfeopiw.html

[R23] 字符串替换
来源：http://hz.sufxvd.cn/gtozrbfcoa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.haohaochexian.top/gtvhfvsddz.html

[R24] 大小写转换
来源：http://hz.aibaodan.cn/gtggqeutoa.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ywan-chungtsiang.top/gtbcnrtzpd.html

[R25] 去后缀 / 去前缀
来源：http://hz.nanxuanxn.top/gtkmueqjjm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.haohaochexian.top/gtiqaczjoi.html

[R26] 命令替换
来源：http://hz.tian-w.cn/gtzzfxpfma.html

now=$(date +%F); echo "$now"
来源：http://hz.hnxiangtu.top/gtejxbuxme.html

[R27] 算术展开
来源：http://hz.hongshengwenyu.top/gtekojsywb.html

echo $((1 + 2 * 3))
来源：http://hz.yuanzhike.top/gtqoaxgmpo.html

[R28] 浮点运算
来源：http://hz.sysykeji.top/gtwxbfualy.html

echo "scale=2; 10/3" | bc
来源：http://hz.ydjk.org.cn/gtismxgqht.html

[R29] 定义函数
来源：http://hz.cashguo.top/gtbornnkla.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yueranfly.top/gtnnggqhzl.html

[R30] 函数返回状态码
来源：http://hz.ydjk.org.cn/gtbytkdtgl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xziqi.cn/gtdjyxwblt.html

[R31] 局部变量
来源：http://hz.andypj.xyz/gtgxuyuzji.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhaomingkeji.xyz/gtwctsthwu.html

[R32] 参数个数校验
来源：http://hz.nanxuanxn.top/gtxokactsd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.316326.xyz/gtwzwvvhce.html

[R33] 捕获错误并提示行号
来源：http://hz.jqgufenzy.top/gtdglpljjx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.snrcjt.cn/gtpnjmqpzs.html

[R34] 退出时清理
来源：http://hz.tianlin.xyz/gtedkfkcdz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinghuilouyu.cn/gtlaeumiht.html

[R35] 后台执行并等待
来源：http://hz.ivvv.top/gtelvhwuvo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.andypj.xyz/gthvoyxwnx.html

[R36] 并发执行多个任务
来源：http://hz.zhixingplan.top/gtjdhlwjzc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yongpay.top/gtjbwrchtt.html

[R37] 把输出赋给变量
来源：http://hz.feifeiyinyue.top/gtjrasldwc.html

files=$(ls -1)
来源：http://hz.shanyushiyangkeji.top/gthylankau.html

[R38] 管道串联
来源：http://hz.jlsjyb.cn/gthcflqupl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.nanxinkj.top/gttosyavbi.html

[R39] 重定向标准输出与错误
来源：http://hz.guowangkeji.top/gtuxkrwvox.html

cmd > out.log 2>&1
来源：http://hz.pycfn.com/gtpsvbousv.html

[R40] 追加写日志
来源：http://hz.fengsongda.top/gtnaywztpz.html

echo "log" >> out.log
来源：http://hz.hysaishi.cn/gtokolxzzy.html

[R41] 丢弃输出
来源：http://hz.hfpthk.cn/gtgwggbbjz.html

cmd >/dev/null 2>&1
来源：http://hz.zhaomingkeji.xyz/gtnxwilozk.html

[R42] 输入重定向
来源：http://hz.quarkkingdee.top/gtwrbmwmbh.html

wc -l < a.txt
来源：http://hz.9152youxi.cn/gtpjjeendh.html

[R43] 按名字查找文件
来源：http://hz.jqgufenzy.top/gtedggvizm.html

find . -name "*.log" -type f
来源：http://hz.smart0.xyz/gtvbqgeabq.html

[R44] 按修改时间查找
来源：http://hz.gzhubu.top/gtcmoxybnz.html

find . -mtime -7 -type f
来源：http://hz.yj20258.top/gtkjadzsmd.html

[R45] 批量删除
来源：http://hz.xingfuxueyuan.xyz/gtekrskzwm.html

find . -name "*.tmp" -delete
来源：http://hz.yongpay.top/gtjkxrsrvs.html

[R46] 递归替换文件内容
来源：http://hz.fzhhl.top/gtqeosnemx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ydzc1.top/gtgjhqeyff.html

[R47] sed 单行替换
来源：http://hz.hysaishi.cn/gtxfleifkq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj202588.top/gtyyninheb.html

[R48] awk 取指定列
来源：http://hz.bjfxy.top/gtriwdeuul.html

awk '{print $1, $3}' a.txt
来源：http://hz.svipenyu.cn/gtkkpryltr.html

[R49] awk 带条件
来源：http://hz.jyoumei.cn/gtwnwacxcl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ybcxt.top/gtrrxlfgjo.html

[R50] awk 求和
来源：http://hz.xylfe.cn/gtpcebysxi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sufxvd.cn/gtkjrodsqg.html

[R51] 排序去重取前几
来源：http://hz.sxryk.cn/gtzmzokjxo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gaohongyu789.top/gtmpecddmu.html

[R52] 统计行数
来源：http://hz.chenjidiqi.icu/gtyjupayed.html

wc -l a.txt
来源：http://hz.daxiang520.top/gtllrikreg.html

[R53] 查看文件头与实时尾
来源：http://hz.zhaomingkeji.xyz/gtlflkejxp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.wangshuangyany.cn/gtyprgpggy.html

[R54] 比较两个文件
来源：http://hz.meibo888.top/gtwvbiwdzg.html

diff a.txt b.txt
来源：http://hz.hnxiangtu.top/gtyxajxbem.html

[R55] 压缩与解压
来源：http://hz.gogol.net.cn/gtvqepsdqn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.feifeiyinyue.top/gtfetqjvgr.html

[R56] 远程拷贝
来源：http://hz.svipenyu.cn/gtsgwpqieg.html

scp file user@host:/path/
来源：http://hz.xingfuxueyuan.xyz/gtlltzrllp.html

[R57] 远程执行命令
来源：http://hz.shzxlz.cn/gtacisdeia.html

ssh user@host 'uptime'
来源：http://hz.yanxiufei.cn/gtyifludgb.html

[R58] 下载文件
来源：http://hz.birdmap.top/gtfasjgaie.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhijiandao.cn/gtcnawhzqg.html

[R59] 发 POST JSON
来源：http://hz.yj20258.top/gtiyhwtloi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jianghu66.top/gttsobvxff.html

[R60] 只看 HTTP 状态码
来源：http://hz.shzxlz.cn/gtdyytsjyc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shangyingyoupin.top/gtabjobjty.html

[R61] 磁盘占用
来源：http://hz.gotoacloud.top/gtfvsbcqqt.html

df -h;  du -sh *
来源：http://hz.haohaochexian.top/gtghxbazoy.html

[R62] 找最占空间的文件
来源：http://hz.cheryme.top/gtcaxismvm.html

du -ah . | sort -rh | head -10
来源：http://hz.dashuyun.cn/gtvbhkoybq.html

[R63] 内存与进程
来源：http://hz.cqqwz.cn/gtyuhiigug.html

free -h;  ps aux | grep nginx
来源：http://hz.hywenlv.cn/gtmmkadxyg.html

[R64] 结束进程
来源：http://hz.hammf.cn/gtdxltpnvn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.pengpengdd.cyou/gteluehhiy.html

[R65] 查看端口占用
来源：http://hz.cucudq.cn/gtytpsftmu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xziqi.cn/gtvpyytusd.html

[R66] 定时任务
来源：http://hz.jinyuanbaomall.cn/gtqrgmqjls.html

crontab -e;  crontab -l
来源：http://hz.hysaishi.cn/gtqdqrpedv.html

[R67] 生成随机十六进制串
来源：http://hz.daxiang520.top/gtusyonptj.html

openssl rand -hex 16
来源：http://hz.jqgufenzy.top/gtmropgjuk.html

[R68] 计算文件校验值
来源：http://hz.jinqigufen.top/gtbseqjvvf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ivvv.top/gturtqzcam.html

[R69] 生成随机密码
来源：http://hz.yanxiufei.cn/gtkdpkkbcy.html

head -c 16 /dev/urandom | base64
来源：http://hz.shanyushiyangtech.top/gtrcgzecxl.html

[R70] 时间戳与互转
来源：http://hz.chenjidiqi.icu/gtrscubipb.html

date +%s;  date -d @1700000000
来源：http://hz.meibo888.top/gtldooehtz.html

[R71] 日期格式化
来源：http://hz.pycfn.com/gtsbgtremf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.fengsongda.top/gtwpddgxup.html

[R72] 等待端口就绪
来源：http://hz.hfpthk.cn/gtipceinht.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.chenlongwang.top/gtwenperpb.html

[R73] 分割大日志
来源：http://hz.chenzaomai.com/gtzhtbbpsz.html

split -l 1000 big.log part_
来源：http://hz.smart0.xyz/gtobdixsei.html

[R74] 批量重命名
来源：http://hz.ydzc1.top/gtwdhzvaov.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xinyue.icu/gtuwkpfjid.html

[R75] 导出环境变量
来源：http://hz.9152youxi.cn/gtwngxacfi.html


<!-- 参考信息 -->