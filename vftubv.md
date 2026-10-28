代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gogol.net.cn/gtgomkeayz.html

[Q22] 排序
来源：http://hz.zdqjudy.top/gtccqpwgtj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.pycfn.com/gtoknhkyod.html

[Q23] 分页
来源：http://hz.yuanzhike.top/gtrremlvda.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.guannengcc.top/gtpcpewsfd.html

[Q24] 去重
来源：http://hz.ydjk.org.cn/gtrxrcqaoh.html

SELECT DISTINCT city FROM users;
来源：http://hz.haohaochexian.top/gtlslgbzot.html

[Q25] 只取前 N 条
来源：http://hz.shzxlz.cn/gtifacuput.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.smart0.xyz/gtuqbojjdz.html

[Q26] 计数
来源：http://hz.zhongyouzk.top/gtggggndla.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtsilxvbqj.html

[Q27] 条件计数
来源：http://hz.sufxvd.cn/gtxzvnyrhj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinqigufen.top/gtligasijl.html

[Q28] 求和与平均
来源：http://hz.meibo888.top/gtncisdtah.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.tianlin.xyz/gtfzunyawa.html

[Q29] 最大最小值
来源：http://hz.quarkkingdee.top/gtanudvwxw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gaohongyu789.top/gtdzdxapwv.html

[Q30] 分组统计
来源：http://hz.jyoumei.cn/gteizebhab.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.fzhhl.top/gtgbwsmksv.html

[Q31] 分组后过滤
来源：http://hz.nanxuanxn.top/gtuahvdftb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhoulong.xyz/gtselulgnc.html

[Q32] 分组拼接字符串
来源：http://hz.cheryme.top/gtprvplpiu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtbtsyqpoo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhiwuduotai.top/gttarooddm.html

[Q33] 多列分组
来源：http://hz.shanyushiyangkeji.top/gtxiutlvru.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ywan-chungtsiang.top/gtymgyvcwf.html

[Q34] 每组取第一条
来源：http://hz.jinqigufen.top/gtgvjtzreb.html

SELECT * FROM (
来源：http://hz.jqgufenzy.top/gtqeygynyk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.pengpengdd.cyou/gtlmtkzevm.html

) t WHERE rn = 1;
来源：http://hz.cucudq.cn/gtuabckvyn.html

[Q35] 内连接
来源：http://hz.chenlongwang.top/gtytcitrcy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ivvv.top/gtnrnpnvqz.html

[Q36] 左连接
来源：http://hz.ydzc1.top/gtthqttieg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ivvv.top/gtbeczrfxe.html

[Q37] 右连接
来源：http://hz.redwolf501.top/gtbamnfxju.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.sxryk.cn/gtrnpddihw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.c1oappe.top/gtifihlrht.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hywenlv.cn/gtzisqouwa.html

[Q39] 自连接（查上下级）
来源：http://hz.shanyushiyangtech.top/gtcmzaefjx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jqgfzy.top/gtpcpzskvm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xuetiantiany.cn/gtpvoqznnv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenjidiqi.icu/gtfuzvnsbs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hfpthk.cn/gtpxrwfqlt.html

[Q41] 多表连接
来源：http://hz.cdnleiting.top/gtnfvgilvw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.pycfn.com/gtgdsedjug.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cucudq.cn/gtccgvmttm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hammf.cn/gtrvbgxyhe.html

[Q42] 连接条件附加过滤
来源：http://hz.havefunace.top/gtamgkoggo.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cheryme.top/gtwxiliimu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hongshengwenyu.top/gtdjpfmmuo.html

[Q43] 标量子查询
来源：http://hz.ivvv.top/gtxzeycchk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shuidangran.top/gtexyzxexe.html

[Q44] IN 子查询
来源：http://hz.iojbl.cn/gtfxzxloky.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.pycfn.com/gtjvujmryd.html

[Q45] EXISTS 判断存在
来源：http://hz.wangdashe.top/gtfqkfahbr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuanzhike.top/gtceezoblg.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ivvv.top/gtkkcrpkdx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jiagoushi.top/gtqnekxiko.html

[Q47] 与平均值比较
来源：http://hz.dashuyun.cn/gthfxelmll.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.meibo888.top/gtytofuenf.html

[Q48] CTE 公用表表达式
来源：http://hz.zhixingplan.top/gtgchckpek.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.mhx1999.top/gttuigqowx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xuanzx.com/gtdreqolid.html

[Q49] 更新单行
来源：http://hz.vqdsnc.cn/gtpcftacpa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenzaomai.com/gtkjomocly.html

[Q50] 批量更新
来源：http://hz.gaohongyu789.top/gtzsxllsob.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ehwqpu.com/gtsgtcihff.html

[Q51] 用子查询更新
来源：http://hz.birdmap.top/gtpuddxvru.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhongyouzk.top/gtwlfxqrod.html

[Q52] 删除指定行
来源：http://hz.ywan-chungtsiang.top/gtxsjrjbby.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gogol.net.cn/gtnmclwamv.html

[Q53] 按条件删除
来源：http://hz.jqgufenzy.top/gtfjcpuuwc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yj20258.top/gtpdwwmfur.html

[Q54] 清空表
来源：http://hz.yonumen.top/gtnailzjvb.html

TRUNCATE TABLE logs;
来源：http://hz.xinyue.icu/gtvipidvay.html

[Q55] 排名（并列占位）
来源：http://hz.yueranfly.top/gteylsdhph.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.9152youxi.cn/gtlmupedxo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.smart0.xyz/gtbbzgmhso.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hongshengwenyu.top/gtazhekvbt.html

[Q57] 行号
来源：http://hz.ppjwa.cn/gtvyytoewo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hammf.cn/gtveblewza.html

[Q58] 累计求和
来源：http://hz.pengpengdd.cyou/gtyttsrmdb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hongshengwenyu.top/gtpglnmmgv.html

[Q59] 分组内累计
来源：http://hz.andypj.xyz/gtkgnkmuzi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhiwuduotai.top/gteexpzten.html

[Q60] 取上一行 / 下一行
来源：http://hz.sysykeji.top/gtolwttnsg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sweek.top/gttwqbhmvx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yuxming.cn/gtvyvyztpi.html

[Q61] 移动平均
来源：http://hz.hywenlv.cn/gtaqrtkiqx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jlsjyb.cn/gtorjodzoi.html

[Q62] 分组占比
来源：http://hz.redwolf501.top/gtkomotyvv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yangfankeji.com/gtyztqgwjj.html

[Q63] 开启事务
来源：http://hz.cucudq.cn/gtkatxzavw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jqgfzy.top/gthvwsyoxv.html

[Q64] 提交事务
来源：http://hz.hysaishi.cn/gtbnfnuxrc.html

COMMIT;
来源：http://hz.redwolf501.top/gtnypzhwhw.html

[Q65] 回滚事务
来源：http://hz.shuidangran.top/gtdujujmqc.html

ROLLBACK;
来源：http://hz.zhiwuduotai.top/gtwojlweju.html

[Q66] 行锁查询
来源：http://hz.mhx1999.top/gtnxyajrkh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shuidangran.top/gtzfobbrli.html

[Q67] 设置隔离级别
来源：http://hz.feifeiyinyue.top/gtaangsxxc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hysaishi.cn/gtnyumpfwq.html

[Q68] 保存点
来源：http://hz.ehwqpu.com/gtxufrpyrz.html

SAVEPOINT sp1;
来源：http://hz.zhijiandao.cn/gttmsfetwy.html

ROLLBACK TO sp1;
来源：http://hz.jqgufenzy.top/gtsvxnvkof.html

[Q69] 查看执行计划
来源：http://hz.xziqi.cn/gttdjhapjx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.c1oappe.top/gtwwriypjn.html

[Q70] 更新统计信息
来源：http://hz.haohaochexian.top/gtxieqeuls.html

ANALYZE TABLE users;
来源：http://hz.sxryk.cn/gtjyeqdnlc.html

[Q71] 查看建表语句
来源：http://hz.chenlongwang.top/gtpvwihanp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ybcxt.top/gtykhgvrxc.html

[Q72] 查看索引
来源：http://hz.ehwqpu.com/gtwncytonq.html

SHOW INDEX FROM users;
来源：http://hz.birdmap.top/gtbrtlynzf.html

[Q73] 查看表状态
来源：http://hz.hnqzz.top/gtksitlpxr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.daxiang520.top/gtohthftjo.html

[Q74] 强制使用索引
来源：http://hz.0kj1m.cn/gtgwjomdhg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.pycfn.com/gtarajwqob.html

[Q75] 日期格式化
来源：http://hz.ydzc1.top/gtyjfraagx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhijiandao.cn/gtmxkewmrq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yuanzhike.top/gtrtdorzyc.html

[Q76] 按天统计
来源：http://hz.dashuyun.cn/gtwkdvueer.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sxryk.cn/gtxxniatdz.html

[Q77] 时间加减
来源：http://hz.c1oappe.top/gtuesknkdc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hywenlv.cn/gtusqeignd.html

[Q78] 当前时间
来源：http://hz.sweek.top/gturmojxnb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hywenlv.cn/gtaclulwmu.html

[Q79] 字符串拼接
来源：http://hz.zhoulong.xyz/gtesxzvrlu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhijiandao.cn/gtroeexdpu.html

[Q80] 字符串截取
来源：http://hz.ehwqpu.com/gttwbxspwj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jqgufenzy.top/gtqybjbmsl.html

[Q81] 字符串替换
来源：http://hz.zhaomingkeji.xyz/gtwqzusfku.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhoulong.xyz/gtysfkxpxe.html

[Q82] 字符长度与字节长度
来源：http://hz.sufxvd.cn/gtzicczsgs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ppjwa.cn/gtpycotyok.html

[Q83] 大小写转换
来源：http://hz.yanxiufei.cn/gtehgifydu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gaohongyu789.top/gtvskrtuip.html

[Q84] 去除首尾空格
来源：http://hz.ehwqpu.com/gturtburpl.html

SELECT TRIM(name) FROM users;
来源：http://hz.hfpthk.cn/gtxkoxhbgo.html

[Q85] 数值取整
来源：http://hz.sysykeji.top/gtkaihyyhe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.0kj1m.cn/gtzqjgitnc.html

[Q86] 读取 JSON 字段
来源：http://hz.wangshuangyany.cn/gtpmqbclvi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tian-w.cn/gtilsftcrr.html

[Q87] JSON 字段做条件
来源：http://hz.guowangkeji.top/gtigjpfxrc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ppjwa.cn/gtjzghwtzk.html

[Q88] 行转列（条件聚合）
来源：http://hz.xuanzx.com/gtfnscljgb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nwbrower.top/gtxfjlldgo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jqgfzy.top/gtlbbkyvab.html

[Q89] 判断表是否存在
来源：http://hz.shangyingyoupin.top/gttsdbvbsz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nwbrower.top/gtghmdohrc.html

[Q90] 生成序号列
来源：http://hz.zhiwuduotai.top/gtmrkdjgcn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.meibo888.top/gtdpcobosj.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtwmqwixso.html

R. Bash 专题
来源：http://hz.wangshuangyany.cn/gtqipisnyp.html

================================================================================
来源：http://hz.mhx1999.top/gteidrwdpm.html

[R01] shebang 与严格模式
来源：http://hz.smart0.xyz/gtikjcmymr.html

#!/usr/bin/env bash
来源：http://hz.jqgufenzy.top/gtspoylwqz.html

set -euo pipefail
来源：http://hz.fzhhl.top/gtpwswkqmg.html

[R02] 变量赋值与使用
来源：http://hz.jinghuilouyu.cn/gthskvpxgf.html

name="Tom"; echo "$name"
来源：http://hz.jqgufenzy.top/gtkfuedxds.html

[R03] 只读变量
来源：http://hz.jqgufenzy.top/gtwvujccvc.html

readonly PI=3.14
来源：http://hz.sweek.top/gtfejmzcor.html

[R04] 位置参数
来源：http://hz.aizwys.cn/gtpiezwtjd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.dashuyun.cn/gtchrfvgdw.html

[R05] 参数默认值
来源：http://hz.sysykeji.top/gtxdaqtwoj.html

name="${1:-default}"
来源：http://hz.aibaodan.cn/gtlrzhetli.html

[R06] 判断命令是否存在
来源：http://hz.iojbl.cn/gtuxbxyhpn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yuxming.cn/gtjmhwtlmc.html

[R07] if 判断文件
来源：http://hz.yanxiufei.cn/gtcwkhzuax.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenjidiqi.icu/gthepfrtir.html

[R08] 数值比较
来源：http://hz.chenzaomai.com/gtdoaadchb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhijiandao.cn/gtuxqirpix.html

[R09] 字符串比较
来源：http://hz.nwbrower.top/gtplgykrdk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yongpay.top/gtokvckzhe.html

[R10] 正则匹配
来源：http://hz.gogol.net.cn/gtbdbhimjr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenzaomai.com/gtjijphdbo.html

[R11] case 多分支
来源：http://hz.yvedp.cn/gtvxxroyef.html

case "$1" in
来源：http://hz.birdmap.top/gtwcmyeicl.html

start) echo "启动" ;;
来源：http://hz.316326.xyz/gtqrfbbasj.html

stop)  echo "停止" ;;
来源：http://hz.kuanghao11.cn/gtsybzwyrq.html

*)     echo "未知命令" ;;
来源：http://hz.wangshuangyany.cn/gtmitcpwmx.html

esac
来源：http://hz.smart0.xyz/gtdaqyphkl.html

[R12] for 遍历文件
来源：http://hz.sufxvd.cn/gtneprfkdi.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jyoumei.cn/gtiellxhdn.html

[R13] for 计数循环
来源：http://hz.tianlin.xyz/gtottpcezy.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.316326.xyz/gtfxetwvra.html

[R14] C 风格 for
来源：http://hz.nanxuanxn.top/gtuokfzrzg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cqqwz.cn/gtdrebhopg.html

[R15] while 逐行读文件
来源：http://hz.wangdashe.top/gtdtltdlhy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.kuanghao11.cn/gtweafzksh.html

[R16] until 等待条件
来源：http://hz.yonumen.top/gtrsijjthi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhaomingkeji.xyz/gtbuowseky.html

[R17] 数组定义与取值
来源：http://hz.cheryme.top/gtvjjszxyw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.iojbl.cn/gtauzrspru.html

[R18] 遍历数组
来源：http://hz.52xcode.cn/gtyhnhbkve.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.vqdsnc.cn/gtfibbjohz.html

[R19] 数组长度
来源：http://hz.jlsjyb.cn/gtnijuengd.html

echo "${#arr[@]}"
来源：http://hz.meibo888.top/gtcaqrzrtl.html

[R20] 关联数组（字典）
来源：http://hz.xinyue.icu/gtfxujkrjc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yonumen.top/gtfwtzgrlq.html

[R21] 字符串长度
来源：http://hz.chenlongwang.top/gtizjfceai.html

echo "${#s}"
来源：http://hz.zhoulong.xyz/gthgopzbhr.html

[R22] 截取子串
来源：http://hz.hammf.cn/gtcadzmmyi.html

echo "${s:0:5}"
来源：http://hz.yvedp.cn/gtqrpahfgg.html

[R23] 字符串替换
来源：http://hz.jqgfzy.top/gtwzkgcrxb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.fengsongda.top/gtnzrgkbsd.html

[R24] 大小写转换
来源：http://hz.shanyushiyangtech.top/gtzgwjukdx.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinqigfzy.top/gtpkpmjkgn.html

[R25] 去后缀 / 去前缀
来源：http://hz.fzhhl.top/gtxocygtjf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xylfe.cn/gtqwbddyer.html

[R26] 命令替换
来源：http://hz.jyoumei.cn/gttmxnjqcp.html

now=$(date +%F); echo "$now"
来源：http://hz.vqdsnc.cn/gtbzckekom.html

[R27] 算术展开
来源：http://hz.daria6918.cn/gtmpkcptcl.html

echo $((1 + 2 * 3))
来源：http://hz.fengsongda.top/gtxfrqtgmn.html

[R28] 浮点运算
来源：http://hz.gzhubu.top/gtbtoonaoy.html

echo "scale=2; 10/3" | bc
来源：http://hz.sweek.top/gtvhmggmiu.html

[R29] 定义函数
来源：http://hz.yvedp.cn/gtrrsutlin.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.daria6918.cn/gtwwxkxeku.html

[R30] 函数返回状态码
来源：http://hz.jianghu66.top/gtbycrdlog.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.mhx1999.top/gthlrjrxhf.html

[R31] 局部变量
来源：http://hz.jinghuilouyu.cn/gtbqyuikju.html

f() { local x=1; echo "$x"; }
来源：http://hz.aizwys.cn/gtjgpezqio.html

[R32] 参数个数校验
来源：http://hz.yuanzhike.top/gtzmshvzbm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.c1oappe.top/gtuhsljagb.html

[R33] 捕获错误并提示行号
来源：http://hz.cucudq.cn/gtjvuiqypq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yongpay.top/gtdickuggn.html

[R34] 退出时清理
来源：http://hz.sxryk.cn/gthvidngch.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtosksfdyz.html

[R35] 后台执行并等待
来源：http://hz.sysykeji.top/gtvvdpsmbz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.fengsongda.top/gtuehjafcj.html

[R36] 并发执行多个任务
来源：http://hz.xuanzx.com/gttuemwltb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zycfv.cn/gttyvlehye.html

[R37] 把输出赋给变量
来源：http://hz.zhengqikj.top/gtuabmonud.html

files=$(ls -1)
来源：http://hz.sufxvd.cn/gtasqgzbgk.html

[R38] 管道串联
来源：http://hz.vqdsnc.cn/gtrievcywn.html

cat a.txt | grep -i error | wc -l
来源：http://hz.feifeiyinyue.top/gtqdhngugu.html

[R39] 重定向标准输出与错误
来源：http://hz.tianlin.xyz/gtazqmdldq.html

cmd > out.log 2>&1
来源：http://hz.ppjwa.cn/gtxqgmptks.html

[R40] 追加写日志
来源：http://hz.zycfv.cn/gtdnzidykz.html

echo "log" >> out.log
来源：http://hz.feifeiyinyue.top/gtttxvddvm.html

[R41] 丢弃输出
来源：http://hz.hongshengwenyu.top/gtidfhatis.html

cmd >/dev/null 2>&1
来源：http://hz.aibaodan.cn/gtbdjnnnvz.html

[R42] 输入重定向
来源：http://hz.316326.xyz/gtwmcayjqf.html

wc -l < a.txt
来源：http://hz.tian-w.cn/gtfgztnewi.html

[R43] 按名字查找文件
来源：http://hz.zhijiandao.cn/gtlsgibrhp.html

find . -name "*.log" -type f
来源：http://hz.xuetiantiany.cn/gtjlwuahdy.html

[R44] 按修改时间查找
来源：http://hz.jinyuanbaomall.cn/gtarazhxvi.html

find . -mtime -7 -type f
来源：http://hz.daxiang520.top/gtqvdgoxgt.html

[R45] 批量删除
来源：http://hz.wangshuangyany.cn/gtrhqnfyvf.html

find . -name "*.tmp" -delete
来源：http://hz.gzhubu.top/gtkgdvsead.html

[R46] 递归替换文件内容
来源：http://hz.daria6918.cn/gtppabbccm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jyoumei.cn/gtvwlpmzqq.html

[R47] sed 单行替换
来源：http://hz.sweek.top/gtueynxolt.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhijiandao.cn/gtbztafkyg.html

[R48] awk 取指定列
来源：http://hz.havefunace.top/gttbdlwres.html

awk '{print $1, $3}' a.txt
来源：http://hz.mhx1999.top/gtspbttrni.html

[R49] awk 带条件
来源：http://hz.ydzc1.top/gtqfpaqzqq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.tanke756.top/gtusweawtb.html

[R50] awk 求和
来源：http://hz.yvedp.cn/gtqwapanrz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hnqzz.top/gtysiyynht.html

[R51] 排序去重取前几
来源：http://hz.mhx1999.top/gttvsebhdr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shanyushiyangtech.top/gthqqvgwrd.html

[R52] 统计行数
来源：http://hz.bjfxy.top/gtjoyrjrgf.html

wc -l a.txt
来源：http://hz.cheryme.top/gtlhwjoymj.html

[R53] 查看文件头与实时尾
来源：http://hz.yueranfly.top/gtfahvousb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.kuanghao11.cn/gtcpvblnnq.html

[R54] 比较两个文件
来源：http://hz.aizwys.cn/gtplktpiwh.html

diff a.txt b.txt
来源：http://hz.zhongyouzk.top/gtayuvsmsv.html

[R55] 压缩与解压
来源：http://hz.wangshuangyany.cn/gtrqhfqtdc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.gotoacloud.top/gtrvxdbwav.html

[R56] 远程拷贝
来源：http://hz.316326.xyz/gtdoqzhjyn.html

scp file user@host:/path/
来源：http://hz.hnxiangtu.top/gtbvakdxvh.html

[R57] 远程执行命令
来源：http://hz.sufxvd.cn/gtytrttapm.html

ssh user@host 'uptime'
来源：http://hz.yj20258888.top/gtycofbioi.html

[R58] 下载文件
来源：http://hz.gogol.net.cn/gtbvplnkiw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhengqikj.top/gtyspdelvl.html

[R59] 发 POST JSON
来源：http://hz.yangfankeji.com/gtlmyuplqk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.aibaodan.cn/gtuxyadeif.html

[R60] 只看 HTTP 状态码
来源：http://hz.aibaodan.cn/gtgmknozhs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gzhubu.top/gtiemqcnhg.html

[R61] 磁盘占用
来源：http://hz.fzhhl.top/gtlfypmuvd.html

df -h;  du -sh *
来源：http://hz.havefunace.top/gtslkkzkyn.html

[R62] 找最占空间的文件
来源：http://hz.hnxiangtu.top/gtzjfmeozw.html

du -ah . | sort -rh | head -10
来源：http://hz.yueranfly.top/gthddoxopm.html

[R63] 内存与进程
来源：http://hz.pycfn.com/gtplozbnxb.html

free -h;  ps aux | grep nginx
来源：http://hz.yonumen.top/gtdqxpwdyp.html

[R64] 结束进程
来源：http://hz.pycfn.com/gtlouevkjs.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenlongwang.top/gtyuctgaya.html

[R65] 查看端口占用
来源：http://hz.zhiwuduotai.top/gtyromegea.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gzhubu.top/gtrpesanrj.html

[R66] 定时任务
来源：http://hz.bjfxy.top/gtwzbldros.html

crontab -e;  crontab -l
来源：http://hz.hnxiangtu.top/gtzwoomnwm.html

[R67] 生成随机十六进制串
来源：http://hz.andypj.xyz/gtmlxhmrmz.html

openssl rand -hex 16
来源：http://hz.316326.xyz/gthklqrnsc.html

[R68] 计算文件校验值
来源：http://hz.feifeiyinyue.top/gthobjlkzq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.smart0.xyz/gtnootdfze.html

[R69] 生成随机密码
来源：http://hz.ppjwa.cn/gtkvlvtxkw.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj20258888.top/gtahyextjn.html

[R70] 时间戳与互转
来源：http://hz.nwbrower.top/gtnbiselyn.html

date +%s;  date -d @1700000000
来源：http://hz.zdqjudy.top/gtytbmfwog.html

[R71] 日期格式化
来源：http://hz.ehwqpu.com/gtiymjkwfr.html


<!-- 参考信息 -->