代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.feifeiyinyue.top/gtgnybqujv.html

[Q26] 计数
来源：http://hz.vqdsnc.cn/gtjnkkinuk.html

SELECT COUNT(*) FROM users;
来源：http://hz.hysaishi.cn/gtfflpyxmu.html

[Q27] 条件计数
来源：http://hz.cdnleiting.top/gtdacelter.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sxryk.cn/gtlzchezll.html

[Q28] 求和与平均
来源：http://hz.shzxlz.cn/gtxtlobqmw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jianghu66.top/gtbnxpbsyo.html

[Q29] 最大最小值
来源：http://hz.nanxuanxn.top/gtcexffizt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xziqi.cn/gtogkbsvcx.html

[Q30] 分组统计
来源：http://hz.zycfv.cn/gtvwyufziq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.nanxuanxn.top/gthqrwjnvs.html

[Q31] 分组后过滤
来源：http://hz.ydzc1.top/gtdaifdfhm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.nanxinkj.top/gtcubajeml.html

[Q32] 分组拼接字符串
来源：http://hz.ydjk.org.cn/gtdmktfaae.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.haohaochexian.top/gteikhabhu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jianghu66.top/gttfdknibg.html

[Q33] 多列分组
来源：http://hz.jiagoushi.top/gterzbkggb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tianlin.xyz/gtphqpfotn.html

[Q34] 每组取第一条
来源：http://hz.xingfuxueyuan.xyz/gtvpjgplby.html

SELECT * FROM (
来源：http://hz.xylfe.cn/gtrwfzrgyx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinqigfzy.top/gtrftvfttq.html

) t WHERE rn = 1;
来源：http://hz.sufxvd.cn/gtvccafpxf.html

[Q35] 内连接
来源：http://hz.xziqi.cn/gtyyusllsj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.daria6918.cn/gtmayqthco.html

[Q36] 左连接
来源：http://hz.smart0.xyz/gtykltjdmy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinqigfzy.top/gtxhnwpbvl.html

[Q37] 右连接
来源：http://hz.zhoulong.xyz/gtdmdurmvc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinyuanbaomall.cn/gtikjihqwj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenlongwang.top/gtzshhzesm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yuanzhike.top/gtljhtchym.html

[Q39] 自连接（查上下级）
来源：http://hz.zhoulong.xyz/gtbfgigayg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.aibaodan.cn/gtpliycsqk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zdqjudy.top/gtqkjxjwem.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhongyouzk.top/gttufuwcqw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.redwolf501.top/gtylkhpmif.html

[Q41] 多表连接
来源：http://hz.shanyushiyangtech.top/gtsfmrxdcr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shanyushiyangkeji.top/gtzqzhdzbh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinyuanbaomall.cn/gtpqervaqf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenzaomai.com/gtcdnavyaj.html

[Q42] 连接条件附加过滤
来源：http://hz.nwbrower.top/gtplefzowf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.aibaodan.cn/gthecrhqrn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shangyingyoupin.top/gtnlfrurew.html

[Q43] 标量子查询
来源：http://hz.xuanzx.com/gtalavatuu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ydjk.org.cn/gtbhhplbti.html

[Q44] IN 子查询
来源：http://hz.tian-w.cn/gtdgdptyur.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yongpay.top/gtdwmccjbi.html

[Q45] EXISTS 判断存在
来源：http://hz.zhongyouzk.top/gturarpoxu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangtech.top/gtcdjqedqv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ivvv.top/gtqkwvyiry.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ppjwa.cn/gtqcliiwnz.html

[Q47] 与平均值比较
来源：http://hz.gogol.net.cn/gtuhoaytzg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.andypj.xyz/gterhlkiiv.html

[Q48] CTE 公用表表达式
来源：http://hz.tanke756.top/gtcnmutkss.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.redwolf501.top/gtcktyumsh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.birdmap.top/gtaxqtfsdn.html

[Q49] 更新单行
来源：http://hz.hywenlv.cn/gtktyvzosr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.guannengcc.top/gtbbwpfbij.html

[Q50] 批量更新
来源：http://hz.nwbrower.top/gtdabvyzbp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.c1oappe.top/gtjmgjqsrz.html

[Q51] 用子查询更新
来源：http://hz.shangyingyoupin.top/gtzttosmpy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenjidiqi.icu/gtnytyukof.html

[Q52] 删除指定行
来源：http://hz.iojbl.cn/gtizromhhc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sysykeji.top/gtnxsjsvbk.html

[Q53] 按条件删除
来源：http://hz.yvedp.cn/gtoysrbfbr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.aizwys.cn/gtgrsdmfkj.html

[Q54] 清空表
来源：http://hz.bjfxy.top/gttvgbmfaj.html

TRUNCATE TABLE logs;
来源：http://hz.sxryk.cn/gtkcbrwdro.html

[Q55] 排名（并列占位）
来源：http://hz.xylfe.cn/gtsudfjtuu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.dianchejie.cn/gtwvslahcz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.redwolf501.top/gtprpftrus.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cqqwz.cn/gthwjvpmwk.html

[Q57] 行号
来源：http://hz.zdqjudy.top/gtpgluhqpw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.fzhhl.top/gtvikttfwm.html

[Q58] 累计求和
来源：http://hz.xylfe.cn/gtdecidmef.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.smart0.xyz/gtfuvdqymu.html

[Q59] 分组内累计
来源：http://hz.hysaishi.cn/gtsrismfdu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xylfe.cn/gtcvkumkls.html

[Q60] 取上一行 / 下一行
来源：http://hz.xylfe.cn/gtshggntlc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sxryk.cn/gtustazaqh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.wangdashe.top/gtpmgonyzs.html

[Q61] 移动平均
来源：http://hz.zhixingplan.top/gtngmmvtcu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.haohaochexian.top/gtfrurebus.html

[Q62] 分组占比
来源：http://hz.bjfxy.top/gtzigywnms.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jianghu66.top/gtofmghtdp.html

[Q63] 开启事务
来源：http://hz.hongshengwenyu.top/gtwdxixmlo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jlsjyb.cn/gtctvxuddn.html

[Q64] 提交事务
来源：http://hz.kuanghao11.cn/gtuzwurkrc.html

COMMIT;
来源：http://hz.yonumen.top/gtkvohkmfd.html

[Q65] 回滚事务
来源：http://hz.aibaodan.cn/gtmbkpnsgc.html

ROLLBACK;
来源：http://hz.yuxming.cn/gtidpytojv.html

[Q66] 行锁查询
来源：http://hz.sufxvd.cn/gtatkkdroa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.316326.xyz/gtsdywehez.html

[Q67] 设置隔离级别
来源：http://hz.nanxinkj.top/gtholjkoji.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.andypj.xyz/gtdwzbdsrh.html

[Q68] 保存点
来源：http://hz.wangdashe.top/gtdchzfqdd.html

SAVEPOINT sp1;
来源：http://hz.hfpthk.cn/gtvnyabbtn.html

ROLLBACK TO sp1;
来源：http://hz.dianchejie.cn/gtamutpvyc.html

[Q69] 查看执行计划
来源：http://hz.hnxiangtu.top/gtxmbolaxe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.dianchejie.cn/gtdfdytrde.html

[Q70] 更新统计信息
来源：http://hz.kuanghao11.cn/gtdfjbppmn.html

ANALYZE TABLE users;
来源：http://hz.aibaodan.cn/gtmbhodpbd.html

[Q71] 查看建表语句
来源：http://hz.fzhhl.top/gtxmkorzsw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.wangdashe.top/gtartxslyy.html

[Q72] 查看索引
来源：http://hz.dashuyun.cn/gtymfwafkf.html

SHOW INDEX FROM users;
来源：http://hz.jlsjyb.cn/gttwlbrnbi.html

[Q73] 查看表状态
来源：http://hz.jlsjyb.cn/gtbcahzfuh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sweek.top/gtldcdzspp.html

[Q74] 强制使用索引
来源：http://hz.vqdsnc.cn/gtstzenyru.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zdqjudy.top/gtitywluap.html

[Q75] 日期格式化
来源：http://hz.hywenlv.cn/gtslnhagsw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jiagoushi.top/gtnvzwdtfe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ehwqpu.com/gtwsrixkqn.html

[Q76] 按天统计
来源：http://hz.daria6918.cn/gtuekltxeo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cdnleiting.top/gthqfcvgtg.html

[Q77] 时间加减
来源：http://hz.zhiwuduotai.top/gtamsizvix.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hnqzz.top/gtvktumiga.html

[Q78] 当前时间
来源：http://hz.cqqwz.cn/gtsetnhvmj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.quarkkingdee.top/gtdziviqdw.html

[Q79] 字符串拼接
来源：http://hz.gotoacloud.top/gtsgcorugc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zycfv.cn/gtbezkhoih.html

[Q80] 字符串截取
来源：http://hz.zhoulong.xyz/gtgtkzjyte.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yanxiufei.cn/gtidqihrgs.html

[Q81] 字符串替换
来源：http://hz.shangyingyoupin.top/gtuzkgwsoo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cheryme.top/gtwfqlinqu.html

[Q82] 字符长度与字节长度
来源：http://hz.svipenyu.cn/gtoyutiale.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.52xcode.cn/gtmvorkfru.html

[Q83] 大小写转换
来源：http://hz.tanke756.top/gthnwmfcjy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yanxiufei.cn/gtfhbasiuj.html

[Q84] 去除首尾空格
来源：http://hz.jqgufenzy.top/gtqtejsaxq.html

SELECT TRIM(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtzhmogjls.html

[Q85] 数值取整
来源：http://hz.aibaodan.cn/gtwrdkomzi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nanxuanxn.top/gtvxwlxrwu.html

[Q86] 读取 JSON 字段
来源：http://hz.zhaomingkeji.xyz/gtgjvoklbz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.pycfn.com/gtkgvnbaxo.html

[Q87] JSON 字段做条件
来源：http://hz.yonumen.top/gtqhjnofdq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhoulong.xyz/gtciwlkcjf.html

[Q88] 行转列（条件聚合）
来源：http://hz.sweek.top/gtkeeqsewo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gaohongyu789.top/gtvqaptgnq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.daxiang520.top/gtwejixbwo.html

[Q89] 判断表是否存在
来源：http://hz.nanxinkj.top/gttozfgoiy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jiagoushi.top/gtxgqxmsjz.html

[Q90] 生成序号列
来源：http://hz.guannengcc.top/gtktiluiqu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yueranfly.top/gtedkcyjzj.html

================================================================================
来源：http://hz.zhijiandao.cn/gthchbixll.html

R. Bash 专题
来源：http://hz.jinyuanbaomall.cn/gtzclcnnpb.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtbyrccpic.html

[R01] shebang 与严格模式
来源：http://hz.tianlin.xyz/gtbmuaqddi.html

#!/usr/bin/env bash
来源：http://hz.nwbrower.top/gtclvkdnxj.html

set -euo pipefail
来源：http://hz.cdnleiting.top/gtnpyhxrhn.html

[R02] 变量赋值与使用
来源：http://hz.shuidangran.top/gttojvjmsy.html

name="Tom"; echo "$name"
来源：http://hz.tanke756.top/gtzovzorvg.html

[R03] 只读变量
来源：http://hz.zhengqikj.top/gtagcoiwly.html

readonly PI=3.14
来源：http://hz.chenlongwang.top/gtmqinpcku.html

[R04] 位置参数
来源：http://hz.zycfv.cn/gtytffstyq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenlongwang.top/gtyhzwlfql.html

[R05] 参数默认值
来源：http://hz.yuxming.cn/gtjdqdggod.html

name="${1:-default}"
来源：http://hz.andypj.xyz/gtjbnsgcpe.html

[R06] 判断命令是否存在
来源：http://hz.jqgfzy.top/gtwyokoksl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hnqzz.top/gtqjkiqonq.html

[R07] if 判断文件
来源：http://hz.bjfxy.top/gtqakamcgx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.fengsongda.top/gtsmgawfbx.html

[R08] 数值比较
来源：http://hz.nwbrower.top/gtaekzhdjp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jqgufenzy.top/gttuxqbonc.html

[R09] 字符串比较
来源：http://hz.chenjidiqi.icu/gthanfeswc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zycfv.cn/gtlvkliyhz.html

[R10] 正则匹配
来源：http://hz.jqgfzy.top/gtjgayqxzf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.andypj.xyz/gtrqaoarse.html

[R11] case 多分支
来源：http://hz.yj20258888.top/gthrpskujr.html

case "$1" in
来源：http://hz.gotoacloud.top/gtjrbwmifw.html

start) echo "启动" ;;
来源：http://hz.gogol.net.cn/gtjouohdjb.html

stop)  echo "停止" ;;
来源：http://hz.yanxiufei.cn/gteubhcbzr.html

*)     echo "未知命令" ;;
来源：http://hz.ybcxt.top/gtgrtyslpq.html

esac
来源：http://hz.jyoumei.cn/gtthexfzqa.html

[R12] for 遍历文件
来源：http://hz.yuanzhike.top/gtlojmeodl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ybcxt.top/gtsxrzjbcv.html

[R13] for 计数循环
来源：http://hz.meibo888.top/gtvggsyaoi.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xziqi.cn/gtvcxxsomw.html

[R14] C 风格 for
来源：http://hz.xinyue.icu/gtmijeoebu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cdnleiting.top/gtkxccyzuv.html

[R15] while 逐行读文件
来源：http://hz.sufxvd.cn/gtsomvxqxx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.quarkkingdee.top/gtgujuewvx.html

[R16] until 等待条件
来源：http://hz.nwbrower.top/gtlwroqvtv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nwbrower.top/gtqoqhgsil.html

[R17] 数组定义与取值
来源：http://hz.zhengqikj.top/gtfcqvotoq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yongpay.top/gtzjknukkd.html

[R18] 遍历数组
来源：http://hz.tian-w.cn/gtakozaegg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.aibaodan.cn/gtfaoqkorm.html

[R19] 数组长度
来源：http://hz.shangyingyoupin.top/gtzvdtgplx.html

echo "${#arr[@]}"
来源：http://hz.jqgufenzy.top/gtkuhsdfzy.html

[R20] 关联数组（字典）
来源：http://hz.shangyingyoupin.top/gtpglhtxsf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tianlin.xyz/gtcyraomxu.html

[R21] 字符串长度
来源：http://hz.jinqigufen.top/gtkefyrsvr.html

echo "${#s}"
来源：http://hz.hammf.cn/gtdulqggeq.html

[R22] 截取子串
来源：http://hz.ivvv.top/gtxebsglhj.html

echo "${s:0:5}"
来源：http://hz.zycfv.cn/gtgsqxkgvs.html

[R23] 字符串替换
来源：http://hz.zhiwuduotai.top/gtwwmnrkdy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jyoumei.cn/gtqshoczkt.html

[R24] 大小写转换
来源：http://hz.zhixingplan.top/gtppcslmlr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258888.top/gthluedbsk.html

[R25] 去后缀 / 去前缀
来源：http://hz.kuanghao11.cn/gtmzftutne.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cqqwz.cn/gtokvcuarj.html

[R26] 命令替换
来源：http://hz.tian-w.cn/gtqoranhcy.html

now=$(date +%F); echo "$now"
来源：http://hz.zycfv.cn/gtosjcajcc.html

[R27] 算术展开
来源：http://hz.mhx1999.top/gtybfbsacf.html

echo $((1 + 2 * 3))
来源：http://hz.nanxuanxn.top/gttbysdxhc.html

[R28] 浮点运算
来源：http://hz.ivvv.top/gtfcrndppg.html

echo "scale=2; 10/3" | bc
来源：http://hz.ivvv.top/gttuyvpvbo.html

[R29] 定义函数
来源：http://hz.52xcode.cn/gtlvxitrfg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.iojbl.cn/gtlrghcmxt.html

[R30] 函数返回状态码
来源：http://hz.mhx1999.top/gtxlvposln.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhixingplan.top/gtmykoyhbz.html

[R31] 局部变量
来源：http://hz.zhixingplan.top/gtzgomorla.html

f() { local x=1; echo "$x"; }
来源：http://hz.ydjk.org.cn/gtekbfphyp.html

[R32] 参数个数校验
来源：http://hz.snrcjt.cn/gtqumghshv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gtmssbabkp.html

[R33] 捕获错误并提示行号
来源：http://hz.pycfn.com/gtbuwsterr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sufxvd.cn/gtcvhlwkqf.html

[R34] 退出时清理
来源：http://hz.shangyingyoupin.top/gtcxywalzw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nwbrower.top/gtkprhyuiq.html

[R35] 后台执行并等待
来源：http://hz.jqgufenzy.top/gtjvtahnzk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.dashuyun.cn/gtlgtgvpeg.html

[R36] 并发执行多个任务
来源：http://hz.iojbl.cn/gtjqrhiddt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.wangshuangyany.cn/gtzxgpvich.html

[R37] 把输出赋给变量
来源：http://hz.shanyushiyangtech.top/gtgofghhqu.html

files=$(ls -1)
来源：http://hz.havefunace.top/gtfzbqaamk.html

[R38] 管道串联
来源：http://hz.zhaomingkeji.xyz/gtvyuhxasf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhijiandao.cn/gtyhplqcrv.html

[R39] 重定向标准输出与错误
来源：http://hz.yueranfly.top/gtdemvfocj.html

cmd > out.log 2>&1
来源：http://hz.ybcxt.top/gtcpvtdsii.html

[R40] 追加写日志
来源：http://hz.shangyingyoupin.top/gtwrrjxksi.html

echo "log" >> out.log
来源：http://hz.yj20258.top/gtqdgmbnzc.html

[R41] 丢弃输出
来源：http://hz.svipenyu.cn/gtohjxahui.html

cmd >/dev/null 2>&1
来源：http://hz.0kj1m.cn/gtvpbwyrcb.html

[R42] 输入重定向
来源：http://hz.jiagoushi.top/gtnpjzmijm.html

wc -l < a.txt
来源：http://hz.tanke756.top/gtwyxaujcn.html

[R43] 按名字查找文件
来源：http://hz.zhijiandao.cn/gthdszjilv.html

find . -name "*.log" -type f
来源：http://hz.nanxinkj.top/gtoefvfbbb.html

[R44] 按修改时间查找
来源：http://hz.cashguo.top/gtzgxpfnwe.html

find . -mtime -7 -type f
来源：http://hz.zhongyouzk.top/gtgjvyghey.html

[R45] 批量删除
来源：http://hz.guowangkeji.top/gtjgbvgyfn.html

find . -name "*.tmp" -delete
来源：http://hz.zycfv.cn/gtfxkgvric.html

[R46] 递归替换文件内容
来源：http://hz.yj20258.top/gtvmdxgxrd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.chenjidiqi.icu/gtqgiqpbnw.html

[R47] sed 单行替换
来源：http://hz.ivvv.top/gtevamvobp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sweek.top/gteymxzilu.html

[R48] awk 取指定列
来源：http://hz.ybcxt.top/gtokhewmzp.html

awk '{print $1, $3}' a.txt
来源：http://hz.cqqwz.cn/gtahwhqkvz.html

[R49] awk 带条件
来源：http://hz.iojbl.cn/gtbeopbpgq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xziqi.cn/gtwfporzpk.html

[R50] awk 求和
来源：http://hz.316326.xyz/gtvlwmqkkt.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gotoacloud.top/gthtkodfff.html

[R51] 排序去重取前几
来源：http://hz.andypj.xyz/gtdznfvkju.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenzaomai.com/gtnircfvta.html

[R52] 统计行数
来源：http://hz.jinyuanbaomall.cn/gtbjgwexvf.html

wc -l a.txt
来源：http://hz.iojbl.cn/gtdbdkslsj.html

[R53] 查看文件头与实时尾
来源：http://hz.zhijiandao.cn/gtudpddqze.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yvedp.cn/gtimgmftdk.html

[R54] 比较两个文件
来源：http://hz.cdnleiting.top/gtkoqfiyot.html

diff a.txt b.txt
来源：http://hz.iojbl.cn/gtwaerordp.html

[R55] 压缩与解压
来源：http://hz.ybcxt.top/gtjynafklr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ydjk.org.cn/gtrtezezfe.html

[R56] 远程拷贝
来源：http://hz.zhiwuduotai.top/gtyeexdmfz.html

scp file user@host:/path/
来源：http://hz.gogol.net.cn/gtaedhnjoh.html

[R57] 远程执行命令
来源：http://hz.redwolf501.top/gtyqjswfjj.html

ssh user@host 'uptime'
来源：http://hz.birdmap.top/gtrxauqomy.html

[R58] 下载文件
来源：http://hz.daxiang520.top/gttskjxwsv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sysykeji.top/gthongwqkm.html

[R59] 发 POST JSON
来源：http://hz.zhengqikj.top/gtzlbjfyxh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.svipenyu.cn/gtdmqlpdpz.html

[R60] 只看 HTTP 状态码
来源：http://hz.52xcode.cn/gtoslfeihw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yuanzhike.top/gtsplmyfsy.html

[R61] 磁盘占用
来源：http://hz.0kj1m.cn/gtszcsnewy.html

df -h;  du -sh *
来源：http://hz.shanyushiyangkeji.top/gtgdghfhqn.html

[R62] 找最占空间的文件
来源：http://hz.shanyushiyangkeji.top/gteuwmorqp.html

du -ah . | sort -rh | head -10
来源：http://hz.9152youxi.cn/gtygfzupyw.html

[R63] 内存与进程
来源：http://hz.dashuyun.cn/gtuupeprfu.html

free -h;  ps aux | grep nginx
来源：http://hz.hongshengwenyu.top/gttgwkizvb.html

[R64] 结束进程
来源：http://hz.aizwys.cn/gtalqewnkd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hongshengwenyu.top/gtvqxzfmot.html

[R65] 查看端口占用
来源：http://hz.mhx1999.top/gtjndzyfut.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.aizwys.cn/gtupwpnyne.html

[R66] 定时任务
来源：http://hz.vqdsnc.cn/gtmlxnixag.html

crontab -e;  crontab -l
来源：http://hz.cqqwz.cn/gtbxhrazxn.html

[R67] 生成随机十六进制串
来源：http://hz.hammf.cn/gtirvhuzjz.html

openssl rand -hex 16
来源：http://hz.yueranfly.top/gtatjuxkws.html

[R68] 计算文件校验值
来源：http://hz.nwbrower.top/gtzunhfcvg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xingfuxueyuan.xyz/gtqmwubmgd.html

[R69] 生成随机密码
来源：http://hz.guannengcc.top/gtqieegdhi.html

head -c 16 /dev/urandom | base64
来源：http://hz.gogol.net.cn/gtmavujpjn.html

[R70] 时间戳与互转
来源：http://hz.hongshengwenyu.top/gtqnnsytaz.html

date +%s;  date -d @1700000000
来源：http://hz.fzhhl.top/gtfilviibh.html

[R71] 日期格式化
来源：http://hz.xuetiantiany.cn/gtqxzuddbs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.daxiang520.top/gtiiqqwhqk.html

[R72] 等待端口就绪
来源：http://hz.nwbrower.top/gtefvanuua.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.quarkkingdee.top/gtjpdyvjok.html

[R73] 分割大日志
来源：http://hz.cqqwz.cn/gterafeaxt.html

split -l 1000 big.log part_
来源：http://hz.ydjk.org.cn/gtdlfdljot.html

[R74] 批量重命名
来源：http://hz.zhaomingkeji.xyz/gtiukquwtk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.quarkkingdee.top/gtbvrnlvfc.html

[R75] 导出环境变量
来源：http://hz.haohaochexian.top/gtbtvwhjdg.html


<!-- 参考信息 -->