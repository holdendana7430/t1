代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.dianchejie.cn/gtdeajcpqs.html

[Q18] 模糊匹配
来源：http://hz.yanxiufei.cn/gtgvrubepm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jqgufenzy.top/gtopgkxewu.html

[Q19] 范围查询
来源：http://hz.xuetiantiany.cn/gtxrlsuvad.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sxryk.cn/gturiphepi.html

[Q20] IN 列表
来源：http://hz.guowangkeji.top/gtlpqtknpa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.dashuyun.cn/gtfcjoauai.html

[Q21] 空值判断
来源：http://hz.ydjk.org.cn/gtxffiksbx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.quarkkingdee.top/gtzzdayjik.html

[Q22] 排序
来源：http://hz.cheryme.top/gtepiexsyn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj202588.top/gtrqvvqrpl.html

[Q23] 分页
来源：http://hz.zhijiandao.cn/gttqakzpjv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.52xcode.cn/gtjmefbxgx.html

[Q24] 去重
来源：http://hz.ywan-chungtsiang.top/gtyzoguzmh.html

SELECT DISTINCT city FROM users;
来源：http://hz.hysaishi.cn/gtiqtrmlah.html

[Q25] 只取前 N 条
来源：http://hz.jqgfzy.top/gtxapqqvdq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.daxiang520.top/gtbaysymly.html

[Q26] 计数
来源：http://hz.ywan-chungtsiang.top/gtjwbblbgj.html

SELECT COUNT(*) FROM users;
来源：http://hz.pycfn.com/gtznmpkvwe.html

[Q27] 条件计数
来源：http://hz.0kj1m.cn/gtuyfszdcj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.bjfxy.top/gtwcvqznnq.html

[Q28] 求和与平均
来源：http://hz.ywan-chungtsiang.top/gtabvqadqh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cashguo.top/gtxuvarnkp.html

[Q29] 最大最小值
来源：http://hz.ivvv.top/gtxsdrxdgt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.wangdashe.top/gtnrqutfyt.html

[Q30] 分组统计
来源：http://hz.andypj.xyz/gteiaxdtji.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gtantmtvht.html

[Q31] 分组后过滤
来源：http://hz.c1oappe.top/gtbboqulim.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hnqzz.top/gtyfjhpzcu.html

[Q32] 分组拼接字符串
来源：http://hz.andypj.xyz/gtoudeotrk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.redwolf501.top/gtdezplbmz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.dianchejie.cn/gtwbinlepp.html

[Q33] 多列分组
来源：http://hz.chenzaomai.com/gtrakpydup.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinqigfzy.top/gtfwzjjout.html

[Q34] 每组取第一条
来源：http://hz.aizwys.cn/gtqlewcbtu.html

SELECT * FROM (
来源：http://hz.bjfxy.top/gtwvdqcayo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zdqjudy.top/gtravkxfls.html

) t WHERE rn = 1;
来源：http://hz.xuetiantiany.cn/gtheuzkfpp.html

[Q35] 内连接
来源：http://hz.cheryme.top/gtywzzdpbx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.feifeiyinyue.top/gthhqkaxpe.html

[Q36] 左连接
来源：http://hz.aizwys.cn/gtfiyhputv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yonumen.top/gtitjfunvb.html

[Q37] 右连接
来源：http://hz.xingfuxueyuan.xyz/gtszfvphlr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.daria6918.cn/gtxyfkydoq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ydjk.org.cn/gtkqibbyvb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gotoacloud.top/gtiwketyaz.html

[Q39] 自连接（查上下级）
来源：http://hz.haohaochexian.top/gtriqjqkei.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.c1oappe.top/gtgzvxfahr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shanyushiyangkeji.top/gtxvyvwnjd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.wangdashe.top/gtprbqlvtc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yonumen.top/gtsuzxucst.html

[Q41] 多表连接
来源：http://hz.wangshuangyany.cn/gtectiunfd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tanke756.top/gtreyhbgtt.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hongshengwenyu.top/gtgspjtznv.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yvedp.cn/gtqifhhznd.html

[Q42] 连接条件附加过滤
来源：http://hz.yuxming.cn/gtvplbtned.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gogol.net.cn/gtopikvedj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.snrcjt.cn/gtxpqfzewv.html

[Q43] 标量子查询
来源：http://hz.cqqwz.cn/gthwecbvlh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.tian-w.cn/gtfawxmrbu.html

[Q44] IN 子查询
来源：http://hz.jqgufenzy.top/gtjhuvvixi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.nanxuanxn.top/gtffnotslu.html

[Q45] EXISTS 判断存在
来源：http://hz.quarkkingdee.top/gtgtpflobr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.c1oappe.top/gtbzgoezle.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xinyue.icu/gtslcdjczt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hfpthk.cn/gtpxzjtzjm.html

[Q47] 与平均值比较
来源：http://hz.tian-w.cn/gtgobevyoc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.mhx1999.top/gtsnwemcqx.html

[Q48] CTE 公用表表达式
来源：http://hz.feifeiyinyue.top/gtudslzisx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.chenlongwang.top/gtalzdcgqr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.birdmap.top/gtvpbeopcs.html

[Q49] 更新单行
来源：http://hz.pycfn.com/gtzjoeadpp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sxryk.cn/gtdslwesiv.html

[Q50] 批量更新
来源：http://hz.yuxming.cn/gtikqpbuff.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yj20258888.top/gtktalvcqd.html

[Q51] 用子查询更新
来源：http://hz.zhiwuduotai.top/gtfpaxuayq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.wangshuangyany.cn/gtwbkclotp.html

[Q52] 删除指定行
来源：http://hz.zhaomingkeji.xyz/gtkafjnadl.html

DELETE FROM users WHERE id = 10;
来源：http://hz.pengpengdd.cyou/gtuhydtgkh.html

[Q53] 按条件删除
来源：http://hz.yueranfly.top/gtgjgiljif.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydjk.org.cn/gtjeihwwoq.html

[Q54] 清空表
来源：http://hz.cucudq.cn/gtiocsdsra.html

TRUNCATE TABLE logs;
来源：http://hz.gogol.net.cn/gtvymztyeh.html

[Q55] 排名（并列占位）
来源：http://hz.ydzc1.top/gtmqeabhpu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinghuilouyu.cn/gtmjrbviky.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xziqi.cn/gthxhofnda.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhongyouzk.top/gtyeivmbva.html

[Q57] 行号
来源：http://hz.yangfankeji.com/gtnymjntys.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xuetiantiany.cn/gtziovlhyv.html

[Q58] 累计求和
来源：http://hz.quarkkingdee.top/gtaqofgddu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.guannengcc.top/gtklckrzlu.html

[Q59] 分组内累计
来源：http://hz.316326.xyz/gtgabpaiua.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nwbrower.top/gtpicnurdu.html

[Q60] 取上一行 / 下一行
来源：http://hz.yonumen.top/gtidvoriro.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.pengpengdd.cyou/gtbzhnygmc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhixingplan.top/gtrcoyqziq.html

[Q61] 移动平均
来源：http://hz.c1oappe.top/gtwgxckfrc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jianghu66.top/gteazyohpq.html

[Q62] 分组占比
来源：http://hz.dashuyun.cn/gtzxfukeyo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtlzkwgpjd.html

[Q63] 开启事务
来源：http://hz.zhoulong.xyz/gtovrvyfgz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shzxlz.cn/gtsojcltgx.html

[Q64] 提交事务
来源：http://hz.guowangkeji.top/gtgvtpmpad.html

COMMIT;
来源：http://hz.xuanzx.com/gtahmkfluv.html

[Q65] 回滚事务
来源：http://hz.daria6918.cn/gtjhnzkqzj.html

ROLLBACK;
来源：http://hz.ydzc1.top/gtughxngcy.html

[Q66] 行锁查询
来源：http://hz.guowangkeji.top/gtrcrgdlnv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yangfankeji.com/gtaaobwgep.html

[Q67] 设置隔离级别
来源：http://hz.c1oappe.top/gtauwbilzn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.0kj1m.cn/gtquejdjkb.html

[Q68] 保存点
来源：http://hz.zhijiandao.cn/gtzdrpxqsv.html

SAVEPOINT sp1;
来源：http://hz.tianlin.xyz/gtvbiqjvvi.html

ROLLBACK TO sp1;
来源：http://hz.jinqigufen.top/gtaindgilo.html

[Q69] 查看执行计划
来源：http://hz.fzhhl.top/gteraepkkv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.svipenyu.cn/gtdrtgjtcm.html

[Q70] 更新统计信息
来源：http://hz.shangyingyoupin.top/gtskeydcrz.html

ANALYZE TABLE users;
来源：http://hz.mhx1999.top/gtfhqtchjg.html

[Q71] 查看建表语句
来源：http://hz.yueranfly.top/gtrqmigqxn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.nanxinkj.top/gttprfpzew.html

[Q72] 查看索引
来源：http://hz.zhaomingkeji.xyz/gtmsjnzapx.html

SHOW INDEX FROM users;
来源：http://hz.52xcode.cn/gtcjpmcltx.html

[Q73] 查看表状态
来源：http://hz.xziqi.cn/gtucpeenpn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shanyushiyangkeji.top/gtdzrixtqb.html

[Q74] 强制使用索引
来源：http://hz.smart0.xyz/gtympivdeg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.wangshuangyany.cn/gtqvvuusbg.html

[Q75] 日期格式化
来源：http://hz.yuanzhike.top/gtacgqtvia.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhongyouzk.top/gtyhdmihws.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.pengpengdd.cyou/gtjywidgvk.html

[Q76] 按天统计
来源：http://hz.bjfxy.top/gtaqueates.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.wangdashe.top/gtvirqjxxt.html

[Q77] 时间加减
来源：http://hz.fzhhl.top/gtsqronaky.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hnxiangtu.top/gtaltkofbk.html

[Q78] 当前时间
来源：http://hz.hfpthk.cn/gtozoocbfa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.tian-w.cn/gtnnhjmxjq.html

[Q79] 字符串拼接
来源：http://hz.jqgufenzy.top/gtudbwtepk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.gzhubu.top/gtocravbla.html

[Q80] 字符串截取
来源：http://hz.fengsongda.top/gthnbispiu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ybcxt.top/gtsipvzgqs.html

[Q81] 字符串替换
来源：http://hz.9152youxi.cn/gtxrhgvoxw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sxryk.cn/gtkootsvkp.html

[Q82] 字符长度与字节长度
来源：http://hz.shanyushiyangtech.top/gtxyfmlixy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.andypj.xyz/gtemjswtlr.html

[Q83] 大小写转换
来源：http://hz.ywan-chungtsiang.top/gtimnxrxyb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tian-w.cn/gthcrprttv.html

[Q84] 去除首尾空格
来源：http://hz.feifeiyinyue.top/gtkpohyqds.html

SELECT TRIM(name) FROM users;
来源：http://hz.shuidangran.top/gtrqmpnmxm.html

[Q85] 数值取整
来源：http://hz.hfpthk.cn/gtatoxdhfh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shangyingyoupin.top/gtclxmijqu.html

[Q86] 读取 JSON 字段
来源：http://hz.hammf.cn/gtmuugugdi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yueranfly.top/gtzvsqyaff.html

[Q87] JSON 字段做条件
来源：http://hz.cheryme.top/gttjnymrsw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.tianlin.xyz/gtokpwcllo.html

[Q88] 行转列（条件聚合）
来源：http://hz.jqgufenzy.top/gtjuqyyewp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ydjk.org.cn/gtgbrfoiww.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cdnleiting.top/gtjbtkkfns.html

[Q89] 判断表是否存在
来源：http://hz.xziqi.cn/gtdqoeoyyr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgufenzy.top/gtarljhbuk.html

[Q90] 生成序号列
来源：http://hz.zhixingplan.top/gtihaxribp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangtech.top/gterrizhdv.html

================================================================================
来源：http://hz.ppjwa.cn/gtqenalcmb.html

R. Bash 专题
来源：http://hz.yvedp.cn/gtxrfkrqsu.html

================================================================================
来源：http://hz.meibo888.top/gtkfxrmure.html

[R01] shebang 与严格模式
来源：http://hz.ehwqpu.com/gtpxkzhbem.html

#!/usr/bin/env bash
来源：http://hz.xingfuxueyuan.xyz/gtaeyfrpny.html

set -euo pipefail
来源：http://hz.yvedp.cn/gturqfvrhk.html

[R02] 变量赋值与使用
来源：http://hz.yongpay.top/gtffoqqyht.html

name="Tom"; echo "$name"
来源：http://hz.yj20258.top/gtruzpebnj.html

[R03] 只读变量
来源：http://hz.bjfxy.top/gtdnmafugo.html

readonly PI=3.14
来源：http://hz.jinqigfzy.top/gtyspkefnw.html

[R04] 位置参数
来源：http://hz.cheryme.top/gtlartpbcz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jlsjyb.cn/gtziebhyyc.html

[R05] 参数默认值
来源：http://hz.svipenyu.cn/gtthlwzuoy.html

name="${1:-default}"
来源：http://hz.xuanzx.com/gtrycuhgsn.html

[R06] 判断命令是否存在
来源：http://hz.daxiang520.top/gtigzyheqe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jlsjyb.cn/gtpnbtxgsx.html

[R07] if 判断文件
来源：http://hz.hfpthk.cn/gtjvifpzje.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.316326.xyz/gtximlttpa.html

[R08] 数值比较
来源：http://hz.havefunace.top/gtoaacdige.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yueranfly.top/gtoyqasdbx.html

[R09] 字符串比较
来源：http://hz.yongpay.top/gttpcpuujb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gaohongyu789.top/gtqbyslvik.html

[R10] 正则匹配
来源：http://hz.yj20258888.top/gtrvsakzim.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.fengsongda.top/gttazydtsu.html

[R11] case 多分支
来源：http://hz.hongshengwenyu.top/gtthtstxys.html

case "$1" in
来源：http://hz.zycfv.cn/gtqnvsybcb.html

start) echo "启动" ;;
来源：http://hz.zhongyouzk.top/gtwqdhjbtw.html

stop)  echo "停止" ;;
来源：http://hz.ivvv.top/gtgipkhlkc.html

*)     echo "未知命令" ;;
来源：http://hz.aibaodan.cn/gtfmtgqzwt.html

esac
来源：http://hz.nanxinkj.top/gtawrnlkyh.html

[R12] for 遍历文件
来源：http://hz.zhengqikj.top/gtrjnbfqgg.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shanyushiyangkeji.top/gtdzstnvdo.html

[R13] for 计数循环
来源：http://hz.svipenyu.cn/gtmwaqjfkb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sweek.top/gtlxteajcy.html

[R14] C 风格 for
来源：http://hz.dianchejie.cn/gtzoalfyqg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nwbrower.top/gtenmrsjhx.html

[R15] while 逐行读文件
来源：http://hz.gotoacloud.top/gtwlmnfytm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sysykeji.top/gtfkldyacg.html

[R16] until 等待条件
来源：http://hz.daxiang520.top/gtjfrnnbmc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ppjwa.cn/gtobkogjpc.html

[R17] 数组定义与取值
来源：http://hz.shzxlz.cn/gtafjvifjh.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sufxvd.cn/gttvrgwhgn.html

[R18] 遍历数组
来源：http://hz.zhiwuduotai.top/gtxifhpkbh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinyuanbaomall.cn/gtdolyrkda.html

[R19] 数组长度
来源：http://hz.shangyingyoupin.top/gtmukafcyt.html

echo "${#arr[@]}"
来源：http://hz.snrcjt.cn/gttdhyetqp.html

[R20] 关联数组（字典）
来源：http://hz.cdnleiting.top/gtphljwfnx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ybcxt.top/gtxhmmwoqr.html

[R21] 字符串长度
来源：http://hz.yuxming.cn/gtdxrqncvx.html

echo "${#s}"
来源：http://hz.yongpay.top/gtxixttuaa.html

[R22] 截取子串
来源：http://hz.sysykeji.top/gtuyffqkxd.html

echo "${s:0:5}"
来源：http://hz.nanxuanxn.top/gtgrqbaskt.html

[R23] 字符串替换
来源：http://hz.cheryme.top/gtziasjhqu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhoulong.xyz/gtkoibvest.html

[R24] 大小写转换
来源：http://hz.shanyushiyangtech.top/gtegtkunix.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhongyouzk.top/gtcyxuvtrx.html

[R25] 去后缀 / 去前缀
来源：http://hz.andypj.xyz/gtaejqqxvh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.snrcjt.cn/gtlbgnxhtn.html

[R26] 命令替换
来源：http://hz.sxryk.cn/gtjrictshr.html

now=$(date +%F); echo "$now"
来源：http://hz.yueranfly.top/gtwcqgmixh.html

[R27] 算术展开
来源：http://hz.9152youxi.cn/gtolioquma.html

echo $((1 + 2 * 3))
来源：http://hz.zhijiandao.cn/gtqxzcjkrn.html

[R28] 浮点运算
来源：http://hz.daxiang520.top/gtdqjvjecj.html

echo "scale=2; 10/3" | bc
来源：http://hz.hongshengwenyu.top/gtqfxuqyqh.html

[R29] 定义函数
来源：http://hz.zhixingplan.top/gtqzfagzif.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guannengcc.top/gtllgtrvqk.html

[R30] 函数返回状态码
来源：http://hz.yangfankeji.com/gtkntakiac.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinyuanbaomall.cn/gttppwazug.html

[R31] 局部变量
来源：http://hz.zhiwuduotai.top/gtxjtplrvh.html

f() { local x=1; echo "$x"; }
来源：http://hz.tianlin.xyz/gtuidmyowc.html

[R32] 参数个数校验
来源：http://hz.daxiang520.top/gtkvisidte.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cqqwz.cn/gtrigxzwrd.html

[R33] 捕获错误并提示行号
来源：http://hz.aibaodan.cn/gtsnnlwyna.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.cashguo.top/gtbucyvhhl.html

[R34] 退出时清理
来源：http://hz.aibaodan.cn/gtkdnhimky.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yangfankeji.com/gtmxgmrick.html

[R35] 后台执行并等待
来源：http://hz.iojbl.cn/gtfffehhis.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xinyue.icu/gtcezegjqr.html

[R36] 并发执行多个任务
来源：http://hz.hfpthk.cn/gtbbaytqdx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhoulong.xyz/gtoslalxix.html

[R37] 把输出赋给变量
来源：http://hz.yj202588.top/gtwsoulyjg.html

files=$(ls -1)
来源：http://hz.cheryme.top/gtvvwgdmxz.html

[R38] 管道串联
来源：http://hz.jinqigufen.top/gtdgfqdavv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ybcxt.top/gtwystgcdm.html

[R39] 重定向标准输出与错误
来源：http://hz.pengpengdd.cyou/gtldibiexq.html

cmd > out.log 2>&1
来源：http://hz.tanke756.top/gtxncddkit.html

[R40] 追加写日志
来源：http://hz.nanxinkj.top/gtvpicpoqc.html

echo "log" >> out.log
来源：http://hz.shanyushiyangkeji.top/gtfedjhygy.html

[R41] 丢弃输出
来源：http://hz.mhx1999.top/gtemljumiu.html

cmd >/dev/null 2>&1
来源：http://hz.jinghuilouyu.cn/gtcfaufqpj.html

[R42] 输入重定向
来源：http://hz.yj20258888.top/gtafpjygyr.html

wc -l < a.txt
来源：http://hz.zhiwuduotai.top/gtsdogrysl.html

[R43] 按名字查找文件
来源：http://hz.xuanzx.com/gtqajttjhk.html

find . -name "*.log" -type f
来源：http://hz.sysykeji.top/gtoofoyqfq.html

[R44] 按修改时间查找
来源：http://hz.zdqjudy.top/gtnaytkumn.html

find . -mtime -7 -type f
来源：http://hz.ehwqpu.com/gtemzuyjlk.html

[R45] 批量删除
来源：http://hz.shangyingyoupin.top/gtlqzdepdy.html

find . -name "*.tmp" -delete
来源：http://hz.meibo888.top/gtamfmuwvy.html

[R46] 递归替换文件内容
来源：http://hz.nanxuanxn.top/gtyorvjxen.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinqigufen.top/gthbxlmtgf.html

[R47] sed 单行替换
来源：http://hz.haohaochexian.top/gtuwqvctiq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fzhhl.top/gtzkqvuqla.html

[R48] awk 取指定列
来源：http://hz.andypj.xyz/gtxmjmvhve.html

awk '{print $1, $3}' a.txt
来源：http://hz.sysykeji.top/gtdzabrfip.html

[R49] awk 带条件
来源：http://hz.mhx1999.top/gtbcxnrjpb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yuxming.cn/gtdqwpmiix.html

[R50] awk 求和
来源：http://hz.yuxming.cn/gteeuexgbu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gzhubu.top/gtnmvqgbhs.html

[R51] 排序去重取前几
来源：http://hz.52xcode.cn/gthgzkewth.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ywan-chungtsiang.top/gtdaagfufj.html

[R52] 统计行数
来源：http://hz.havefunace.top/gtadzlyrwo.html

wc -l a.txt
来源：http://hz.shanyushiyangkeji.top/gthpegayxk.html

[R53] 查看文件头与实时尾
来源：http://hz.yueranfly.top/gtlsegohys.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cqqwz.cn/gtrjpsewzq.html

[R54] 比较两个文件
来源：http://hz.nwbrower.top/gtrponivab.html

diff a.txt b.txt
来源：http://hz.zhongyouzk.top/gtkhgfptdd.html

[R55] 压缩与解压
来源：http://hz.shanyushiyangtech.top/gtiaaypnny.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.redwolf501.top/gtxgvvzark.html

[R56] 远程拷贝
来源：http://hz.ydjk.org.cn/gttdplikct.html

scp file user@host:/path/
来源：http://hz.xziqi.cn/gtyufigwdn.html

[R57] 远程执行命令
来源：http://hz.chenlongwang.top/gtdjwdiaip.html

ssh user@host 'uptime'
来源：http://hz.wangdashe.top/gturgdzvig.html

[R58] 下载文件
来源：http://hz.316326.xyz/gtjlcnpruz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj20258.top/gtkusgdwko.html

[R59] 发 POST JSON
来源：http://hz.birdmap.top/gtemlzgshd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yanxiufei.cn/gtscvmbfld.html

[R60] 只看 HTTP 状态码
来源：http://hz.redwolf501.top/gtkzxelygj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.dianchejie.cn/gthfvofwps.html

[R61] 磁盘占用
来源：http://hz.tianlin.xyz/gtukwplsbq.html

df -h;  du -sh *
来源：http://hz.shanyushiyangkeji.top/gtfanpjrhu.html

[R62] 找最占空间的文件
来源：http://hz.hammf.cn/gtbgabeekd.html

du -ah . | sort -rh | head -10
来源：http://hz.jyoumei.cn/gtdcadvveq.html

[R63] 内存与进程
来源：http://hz.yonumen.top/gtplnwekti.html

free -h;  ps aux | grep nginx
来源：http://hz.andypj.xyz/gtalqbhwpp.html

[R64] 结束进程
来源：http://hz.hfpthk.cn/gtszyqtthf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigfzy.top/gtqlypyjqz.html

[R65] 查看端口占用
来源：http://hz.yj20258888.top/gtqymgoeec.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hnxiangtu.top/gtvzviirpm.html

[R66] 定时任务
来源：http://hz.ywan-chungtsiang.top/gtampzpjjs.html

crontab -e;  crontab -l
来源：http://hz.tianlin.xyz/gtxxwidtyk.html

[R67] 生成随机十六进制串
来源：http://hz.yj20258888.top/gtaltuwqfq.html


<!-- 参考信息 -->