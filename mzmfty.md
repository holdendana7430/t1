代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.quarkkingdee.top/gtueevtncw.html

[Q20] IN 列表
来源：http://hz.jqgufenzy.top/gtinqybzlg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cashguo.top/gtlcptjxpb.html

[Q21] 空值判断
来源：http://hz.zhaomingkeji.xyz/gtdkkocpai.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhengqikj.top/gtifvlapvb.html

[Q22] 排序
来源：http://hz.gaohongyu789.top/gtgveklirf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.guannengcc.top/gtxjaziquq.html

[Q23] 分页
来源：http://hz.zhaomingkeji.xyz/gtyeazetgg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yj20258.top/gtaihkctjg.html

[Q24] 去重
来源：http://hz.yuxming.cn/gtvgmdixbs.html

SELECT DISTINCT city FROM users;
来源：http://hz.wangdashe.top/gtxzyicidr.html

[Q25] 只取前 N 条
来源：http://hz.chenjidiqi.icu/gtomcvisec.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jqgfzy.top/gtfbbayfbr.html

[Q26] 计数
来源：http://hz.gzhubu.top/gtorqwllpj.html

SELECT COUNT(*) FROM users;
来源：http://hz.jiagoushi.top/gtfrglyhpb.html

[Q27] 条件计数
来源：http://hz.yj202588.top/gttmljfkrp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shzxlz.cn/gtbdefbipz.html

[Q28] 求和与平均
来源：http://hz.ybcxt.top/gtukzwtplb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jiagoushi.top/gturguwbsi.html

[Q29] 最大最小值
来源：http://hz.tianlin.xyz/gtahqikfyo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.quarkkingdee.top/gtkwdldeug.html

[Q30] 分组统计
来源：http://hz.dashuyun.cn/gtqyqxgoav.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sufxvd.cn/gtsnrcpgyx.html

[Q31] 分组后过滤
来源：http://hz.dianchejie.cn/gtpzyhywih.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yueranfly.top/gtoqfcczlp.html

[Q32] 分组拼接字符串
来源：http://hz.zdqjudy.top/gtrallhxge.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.dashuyun.cn/gtlhanasjg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jiagoushi.top/gthmbmazet.html

[Q33] 多列分组
来源：http://hz.jiagoushi.top/gtbxcguavz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.havefunace.top/gtprlnjbhg.html

[Q34] 每组取第一条
来源：http://hz.feifeiyinyue.top/gtmxkdxqkj.html

SELECT * FROM (
来源：http://hz.hfpthk.cn/gtyqtczddh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jqgufenzy.top/gtqagdndyp.html

) t WHERE rn = 1;
来源：http://hz.tianlin.xyz/gtikwmdzqh.html

[Q35] 内连接
来源：http://hz.xingfuxueyuan.xyz/gtbcmjiwtg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhengqikj.top/gtvnsuqnes.html

[Q36] 左连接
来源：http://hz.nanxinkj.top/gtvkwvivug.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhijiandao.cn/gtbivbmrox.html

[Q37] 右连接
来源：http://hz.yanxiufei.cn/gtskpoxrld.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cqqwz.cn/gtvtqjzcdj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.feifeiyinyue.top/gtlmbqrwxy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zdqjudy.top/gthyukougv.html

[Q39] 自连接（查上下级）
来源：http://hz.cqqwz.cn/gtwheonuxa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinyuanbaomall.cn/gtizoltqdd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.snrcjt.cn/gtdzmeqstd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.fzhhl.top/gtwsvavgzr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.tian-w.cn/gtakhhtozp.html

[Q41] 多表连接
来源：http://hz.cheryme.top/gtrghjbazy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhijiandao.cn/gtmxsahvfq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ybcxt.top/gtokoevyet.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.iojbl.cn/gtxruyyxcr.html

[Q42] 连接条件附加过滤
来源：http://hz.quarkkingdee.top/gtvipbtqiy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.andypj.xyz/gtmiwhqfgw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.chenzaomai.com/gtsgnrgcex.html

[Q43] 标量子查询
来源：http://hz.hfpthk.cn/gtohhwsuar.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jyoumei.cn/gtnwracxuu.html

[Q44] IN 子查询
来源：http://hz.xuetiantiany.cn/gtqaugaccl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yangfankeji.com/gtumdnwkvc.html

[Q45] EXISTS 判断存在
来源：http://hz.cheryme.top/gtlnqmdfnf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhijiandao.cn/gteysgxabq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jianghu66.top/gtewkkpqcs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuanzhike.top/gtfimowehr.html

[Q47] 与平均值比较
来源：http://hz.daxiang520.top/gtjaetlytn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhengqikj.top/gtswknpbmr.html

[Q48] CTE 公用表表达式
来源：http://hz.yj202588.top/gtuihsbyar.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xingfuxueyuan.xyz/gtzdcnosjl.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhijiandao.cn/gtcfzbujzb.html

[Q49] 更新单行
来源：http://hz.shzxlz.cn/gtfkgqvdvc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.redwolf501.top/gtxqmmcmxi.html

[Q50] 批量更新
来源：http://hz.jianghu66.top/gtvlvkgxev.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shanyushiyangkeji.top/gtxbwpqdes.html

[Q51] 用子查询更新
来源：http://hz.9152youxi.cn/gtebpqldsw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.haohaochexian.top/gtgahyeiij.html

[Q52] 删除指定行
来源：http://hz.iojbl.cn/gtwmibyfmj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.wangshuangyany.cn/gtzonsikeh.html

[Q53] 按条件删除
来源：http://hz.yuxming.cn/gtkbjjluai.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhixingplan.top/gtjercvnps.html

[Q54] 清空表
来源：http://hz.pycfn.com/gtkszatrik.html

TRUNCATE TABLE logs;
来源：http://hz.cashguo.top/gtjgljvjcs.html

[Q55] 排名（并列占位）
来源：http://hz.daxiang520.top/gtmtxpsbes.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.daxiang520.top/gtxnvyrezu.html

[Q56] 密集排名（并列不占位）
来源：http://hz.guannengcc.top/gthlimgwhk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shangyingyoupin.top/gtejxrryps.html

[Q57] 行号
来源：http://hz.kuanghao11.cn/gtwflvpsdk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.tianlin.xyz/gtxdrqpssh.html

[Q58] 累计求和
来源：http://hz.cashguo.top/gtjcyyiaky.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hfpthk.cn/gtydcucdfl.html

[Q59] 分组内累计
来源：http://hz.52xcode.cn/gtoqwmwytx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.dianchejie.cn/gtpuvlvdhp.html

[Q60] 取上一行 / 下一行
来源：http://hz.hnqzz.top/gtzkffndqs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.pycfn.com/gtqkovpogx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.wangshuangyany.cn/gtxtabtulo.html

[Q61] 移动平均
来源：http://hz.zhengqikj.top/gttmuigdnt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgfzy.top/gtckybnmnh.html

[Q62] 分组占比
来源：http://hz.nwbrower.top/gtdssuevpr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenlongwang.top/gtqglhqwwe.html

[Q63] 开启事务
来源：http://hz.zdqjudy.top/gtyybfflmc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cheryme.top/gtcqomfszk.html

[Q64] 提交事务
来源：http://hz.yj20258.top/gtrhirldwl.html

COMMIT;
来源：http://hz.wangdashe.top/gtvehvyoxj.html

[Q65] 回滚事务
来源：http://hz.shanyushiyangkeji.top/gtlrqtfcux.html

ROLLBACK;
来源：http://hz.zhijiandao.cn/gtdbzankqt.html

[Q66] 行锁查询
来源：http://hz.zdqjudy.top/gtkswblqqj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhixingplan.top/gtowdjclpx.html

[Q67] 设置隔离级别
来源：http://hz.gotoacloud.top/gtszfacgqc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xuanzx.com/gtsnydxkut.html

[Q68] 保存点
来源：http://hz.jinqigufen.top/gtcbwlabyx.html

SAVEPOINT sp1;
来源：http://hz.zhoulong.xyz/gtxrzpktqp.html

ROLLBACK TO sp1;
来源：http://hz.haohaochexian.top/gtcsgntjgc.html

[Q69] 查看执行计划
来源：http://hz.chenjidiqi.icu/gtyuacrnbw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jqgfzy.top/gttvwqxsrz.html

[Q70] 更新统计信息
来源：http://hz.jqgufenzy.top/gtogvlmjjn.html

ANALYZE TABLE users;
来源：http://hz.c1oappe.top/gtlbpxrlrn.html

[Q71] 查看建表语句
来源：http://hz.zhixingplan.top/gthwrtgaqz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenjidiqi.icu/gtmvpdijof.html

[Q72] 查看索引
来源：http://hz.daxiang520.top/gtzjwhuelg.html

SHOW INDEX FROM users;
来源：http://hz.wangdashe.top/gtcbqngvnw.html

[Q73] 查看表状态
来源：http://hz.jinyuanbaomall.cn/gtmwkzguzp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhixingplan.top/gtgcdfwhwp.html

[Q74] 强制使用索引
来源：http://hz.hywenlv.cn/gtpbxjzayc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tanke756.top/gtvvngzkkm.html

[Q75] 日期格式化
来源：http://hz.gogol.net.cn/gtyseejwfc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtaelzdrqr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.aizwys.cn/gtmujyrchw.html

[Q76] 按天统计
来源：http://hz.pycfn.com/gtftdomgjt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhoulong.xyz/gtarvtxtru.html

[Q77] 时间加减
来源：http://hz.gotoacloud.top/gtvvhyqilh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yj20258888.top/gtzrmqkhvd.html

[Q78] 当前时间
来源：http://hz.sufxvd.cn/gtzjdbtagt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yvedp.cn/gtceiwbuwq.html

[Q79] 字符串拼接
来源：http://hz.bjfxy.top/gttabsjxkb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.pycfn.com/gtqacvfyzh.html

[Q80] 字符串截取
来源：http://hz.cucudq.cn/gtkqlswela.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.fengsongda.top/gtinlbatsq.html

[Q81] 字符串替换
来源：http://hz.quarkkingdee.top/gteyhoecfj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jianghu66.top/gthkcdoftn.html

[Q82] 字符长度与字节长度
来源：http://hz.hnxiangtu.top/gtsrfovtus.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.aibaodan.cn/gtjrryfsqr.html

[Q83] 大小写转换
来源：http://hz.yj20258.top/gtcgmcgkpl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.52xcode.cn/gtxsqupqcv.html

[Q84] 去除首尾空格
来源：http://hz.dianchejie.cn/gtakjxhlzu.html

SELECT TRIM(name) FROM users;
来源：http://hz.ehwqpu.com/gtrcynsxqe.html

[Q85] 数值取整
来源：http://hz.cqqwz.cn/gtzpnjwtdf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zycfv.cn/gtitkxqpwi.html

[Q86] 读取 JSON 字段
来源：http://hz.shanyushiyangkeji.top/gteaplrdgc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.dianchejie.cn/gtispegjdc.html

[Q87] JSON 字段做条件
来源：http://hz.zhaomingkeji.xyz/gtwvsmvxxp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xuanzx.com/gtjrgoicir.html

[Q88] 行转列（条件聚合）
来源：http://hz.tian-w.cn/gtoaljitqe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yj202588.top/gtzzvywpri.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.dianchejie.cn/gtiugperha.html

[Q89] 判断表是否存在
来源：http://hz.gogol.net.cn/gtntqksjml.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.andypj.xyz/gtyupbhyrm.html

[Q90] 生成序号列
来源：http://hz.zhoulong.xyz/gttcyqtowt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gzhubu.top/gtkfrcgvpu.html

================================================================================
来源：http://hz.yueranfly.top/gtuxaflolm.html

R. Bash 专题
来源：http://hz.yonumen.top/gthczqtuqb.html

================================================================================
来源：http://hz.daxiang520.top/gtktrcgngw.html

[R01] shebang 与严格模式
来源：http://hz.meibo888.top/gtmokyovhb.html

#!/usr/bin/env bash
来源：http://hz.guowangkeji.top/gtohgghfew.html

set -euo pipefail
来源：http://hz.shanyushiyangtech.top/gtvqtmberh.html

[R02] 变量赋值与使用
来源：http://hz.jinqigufen.top/gtxsthgema.html

name="Tom"; echo "$name"
来源：http://hz.gogol.net.cn/gtnbpilggb.html

[R03] 只读变量
来源：http://hz.cqqwz.cn/gtrwmqupxw.html

readonly PI=3.14
来源：http://hz.yj20258888.top/gtowbmvwza.html

[R04] 位置参数
来源：http://hz.jqgufenzy.top/gtskglbmos.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yonumen.top/gtwjjxfsiz.html

[R05] 参数默认值
来源：http://hz.zhiwuduotai.top/gtpqfbwfxg.html

name="${1:-default}"
来源：http://hz.quarkkingdee.top/gtyhlgfbfi.html

[R06] 判断命令是否存在
来源：http://hz.kuanghao11.cn/gtwdgsqqip.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.wangshuangyany.cn/gtuccpyvba.html

[R07] if 判断文件
来源：http://hz.pycfn.com/gtxnfrdpkh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.birdmap.top/gtyrvlwrdx.html

[R08] 数值比较
来源：http://hz.hongshengwenyu.top/gtjznjkhgn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.fzhhl.top/gtvszbhoxr.html

[R09] 字符串比较
来源：http://hz.gotoacloud.top/gtrswuytsc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.iojbl.cn/gtsytpcvgs.html

[R10] 正则匹配
来源：http://hz.ppjwa.cn/gtapttnooa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tian-w.cn/gtkxlmgetd.html

[R11] case 多分支
来源：http://hz.chenzaomai.com/gtztoejmld.html

case "$1" in
来源：http://hz.gogol.net.cn/gtjuzfxhmi.html

start) echo "启动" ;;
来源：http://hz.bjfxy.top/gtkjyendwv.html

stop)  echo "停止" ;;
来源：http://hz.jinqigfzy.top/gtgadimzup.html

*)     echo "未知命令" ;;
来源：http://hz.zdqjudy.top/gthzyroxmx.html

esac
来源：http://hz.fengsongda.top/gtrxnwnllf.html

[R12] for 遍历文件
来源：http://hz.yuanzhike.top/gtjdnesnuz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ppjwa.cn/gthhdydvtv.html

[R13] for 计数循环
来源：http://hz.yueranfly.top/gtwhkmadmp.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ybcxt.top/gtajlkeqvy.html

[R14] C 风格 for
来源：http://hz.ydzc1.top/gtunymsscc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.quarkkingdee.top/gtafiawmxl.html

[R15] while 逐行读文件
来源：http://hz.zycfv.cn/gtqyamsmhf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.0kj1m.cn/gtjsoyyjum.html

[R16] until 等待条件
来源：http://hz.jinghuilouyu.cn/gtoqrtvuqm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.316326.xyz/gtbevgyuoy.html

[R17] 数组定义与取值
来源：http://hz.zhixingplan.top/gtmaalqwzu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ivvv.top/gtnqofnbzs.html

[R18] 遍历数组
来源：http://hz.yj20258.top/gtgesntqlv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.haohaochexian.top/gtczknckeq.html

[R19] 数组长度
来源：http://hz.gaohongyu789.top/gtxuawrbau.html

echo "${#arr[@]}"
来源：http://hz.jlsjyb.cn/gtqvagpngt.html

[R20] 关联数组（字典）
来源：http://hz.hywenlv.cn/gtxphnlelm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhoulong.xyz/gtvspyrjtw.html

[R21] 字符串长度
来源：http://hz.dashuyun.cn/gtwxloesra.html

echo "${#s}"
来源：http://hz.wangdashe.top/gtfsvgebij.html

[R22] 截取子串
来源：http://hz.chenzaomai.com/gtwyygvasd.html

echo "${s:0:5}"
来源：http://hz.hywenlv.cn/gtkylbukvq.html

[R23] 字符串替换
来源：http://hz.xziqi.cn/gtpvehwgrb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yonumen.top/gtghrgksnc.html

[R24] 大小写转换
来源：http://hz.haohaochexian.top/gtvlxgwwri.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.guowangkeji.top/gtlwmzzgpp.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhijiandao.cn/gtbxfugjnh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.iojbl.cn/gtkgopofel.html

[R26] 命令替换
来源：http://hz.ybcxt.top/gthqeuqxdq.html

now=$(date +%F); echo "$now"
来源：http://hz.yj20258888.top/gtdsilagow.html

[R27] 算术展开
来源：http://hz.sweek.top/gtuqlpwcys.html

echo $((1 + 2 * 3))
来源：http://hz.tian-w.cn/gtgiokfynd.html

[R28] 浮点运算
来源：http://hz.dashuyun.cn/gtyabtyevs.html

echo "scale=2; 10/3" | bc
来源：http://hz.tian-w.cn/gtobjvinoz.html

[R29] 定义函数
来源：http://hz.zhongyouzk.top/gtshzoluqt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ydzc1.top/gttkaudcgy.html

[R30] 函数返回状态码
来源：http://hz.jianghu66.top/gtidgsjrcc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.c1oappe.top/gtjmgltxcp.html

[R31] 局部变量
来源：http://hz.jinyuanbaomall.cn/gtatdjcdke.html

f() { local x=1; echo "$x"; }
来源：http://hz.aizwys.cn/gtdrnawzbj.html

[R32] 参数个数校验
来源：http://hz.birdmap.top/gtublfixet.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhaomingkeji.xyz/gtkcqxgwuq.html

[R33] 捕获错误并提示行号
来源：http://hz.hnxiangtu.top/gtmyobcaof.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigfzy.top/gtoxtbkzhy.html

[R34] 退出时清理
来源：http://hz.jianghu66.top/gtqiymmait.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhixingplan.top/gtxfylgxof.html

[R35] 后台执行并等待
来源：http://hz.cdnleiting.top/gtfhkwtged.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.daxiang520.top/gtxeyqpubp.html

[R36] 并发执行多个任务
来源：http://hz.xuetiantiany.cn/gtkyyvouki.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.pycfn.com/gtkehildec.html

[R37] 把输出赋给变量
来源：http://hz.pycfn.com/gtmuxyhikr.html

files=$(ls -1)
来源：http://hz.shuidangran.top/gtchyumial.html

[R38] 管道串联
来源：http://hz.redwolf501.top/gthtcoskcj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.havefunace.top/gtmgbmkdbc.html

[R39] 重定向标准输出与错误
来源：http://hz.shanyushiyangkeji.top/gtsfyirsjn.html

cmd > out.log 2>&1
来源：http://hz.ydjk.org.cn/gtmfwxedbl.html

[R40] 追加写日志
来源：http://hz.xingfuxueyuan.xyz/gtmwofbwyv.html

echo "log" >> out.log
来源：http://hz.xylfe.cn/gtfzpndgbg.html

[R41] 丢弃输出
来源：http://hz.tianlin.xyz/gtzwfzdlvo.html

cmd >/dev/null 2>&1
来源：http://hz.redwolf501.top/gttkloluyh.html

[R42] 输入重定向
来源：http://hz.zdqjudy.top/gtbwnkeipz.html

wc -l < a.txt
来源：http://hz.ehwqpu.com/gtpkqpedov.html

[R43] 按名字查找文件
来源：http://hz.jyoumei.cn/gtibyuvdgx.html

find . -name "*.log" -type f
来源：http://hz.cqqwz.cn/gtrhxtrbyr.html

[R44] 按修改时间查找
来源：http://hz.jinqigfzy.top/gtjhpjrvru.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangkeji.top/gtbfclgsea.html

[R45] 批量删除
来源：http://hz.ybcxt.top/gtlllzbscp.html

find . -name "*.tmp" -delete
来源：http://hz.ppjwa.cn/gtpjcnhbbi.html

[R46] 递归替换文件内容
来源：http://hz.nanxinkj.top/gtqcunjmig.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhengqikj.top/gtncbabvur.html

[R47] sed 单行替换
来源：http://hz.snrcjt.cn/gtfkgpdxeu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.iojbl.cn/gtyhgauxxx.html

[R48] awk 取指定列
来源：http://hz.wangshuangyany.cn/gtlmdvagse.html

awk '{print $1, $3}' a.txt
来源：http://hz.wangshuangyany.cn/gtidmdyeru.html

[R49] awk 带条件
来源：http://hz.quarkkingdee.top/gtlauztctw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhixingplan.top/gtpbsshllm.html

[R50] awk 求和
来源：http://hz.ywan-chungtsiang.top/gtnjjfbaaf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenzaomai.com/gttjitrxht.html

[R51] 排序去重取前几
来源：http://hz.ydjk.org.cn/gtacaiemaw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sysykeji.top/gtormmhvth.html

[R52] 统计行数
来源：http://hz.dianchejie.cn/gtzikoexfk.html

wc -l a.txt
来源：http://hz.snrcjt.cn/gthdsjmjfr.html

[R53] 查看文件头与实时尾
来源：http://hz.yongpay.top/gtozujuola.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cheryme.top/gtzlyofmas.html

[R54] 比较两个文件
来源：http://hz.daxiang520.top/gtnzwuwbav.html

diff a.txt b.txt
来源：http://hz.chenzaomai.com/gtcbncufvt.html

[R55] 压缩与解压
来源：http://hz.kuanghao11.cn/gttqckhvhn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.redwolf501.top/gticxyrmvp.html

[R56] 远程拷贝
来源：http://hz.kuanghao11.cn/gthkzlgpdg.html

scp file user@host:/path/
来源：http://hz.bjfxy.top/gtsyncrksm.html

[R57] 远程执行命令
来源：http://hz.guowangkeji.top/gtdpodskoz.html

ssh user@host 'uptime'
来源：http://hz.pycfn.com/gtylhpsdmh.html

[R58] 下载文件
来源：http://hz.gaohongyu789.top/gtgwwtbcbu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenzaomai.com/gtjzqjftmm.html

[R59] 发 POST JSON
来源：http://hz.andypj.xyz/gtjnctcrth.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.meibo888.top/gtepocilyj.html

[R60] 只看 HTTP 状态码
来源：http://hz.andypj.xyz/gtehmabttx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.daxiang520.top/gtitwfsszv.html

[R61] 磁盘占用
来源：http://hz.fengsongda.top/gttbbzsviu.html

df -h;  du -sh *
来源：http://hz.yj20258888.top/gtutjvcyfk.html

[R62] 找最占空间的文件
来源：http://hz.wangdashe.top/gtawcmvutc.html

du -ah . | sort -rh | head -10
来源：http://hz.ehwqpu.com/gtlszyaeib.html

[R63] 内存与进程
来源：http://hz.aizwys.cn/gtiwrmiddc.html

free -h;  ps aux | grep nginx
来源：http://hz.cqqwz.cn/gtnwlvwavw.html

[R64] 结束进程
来源：http://hz.shanyushiyangtech.top/gtkgbkzmim.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zycfv.cn/gthxeocwgn.html

[R65] 查看端口占用
来源：http://hz.quarkkingdee.top/gtuyjcqseg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.quarkkingdee.top/gtjqyjrqnw.html

[R66] 定时任务
来源：http://hz.cashguo.top/gtzwbboowj.html

crontab -e;  crontab -l
来源：http://hz.cashguo.top/gtwpdaflxo.html

[R67] 生成随机十六进制串
来源：http://hz.quarkkingdee.top/gtqulofrdn.html

openssl rand -hex 16
来源：http://hz.shzxlz.cn/gtgitrdmhr.html

[R68] 计算文件校验值
来源：http://hz.iojbl.cn/gtfxbwpajd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yangfankeji.com/gtoqjzbdla.html

[R69] 生成随机密码
来源：http://hz.kuanghao11.cn/gtjbfimaxb.html


<!-- 参考信息 -->