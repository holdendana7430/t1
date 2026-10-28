代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.kuanghao11.cn/gtjqdjgobk.html

[Q30] 分组统计
来源：http://hz.ybcxt.top/gtrcdrkhzr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtxbzrupnr.html

[Q31] 分组后过滤
来源：http://hz.guannengcc.top/gtpcflqojm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jianghu66.top/gtocdwpudi.html

[Q32] 分组拼接字符串
来源：http://hz.meibo888.top/gtbllsgvnt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtqkjaevwc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ybcxt.top/gtmjhhirjp.html

[Q33] 多列分组
来源：http://hz.jlsjyb.cn/gtgseneels.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gogol.net.cn/gtfsaldmfv.html

[Q34] 每组取第一条
来源：http://hz.jinyuanbaomall.cn/gtlyycfzhl.html

SELECT * FROM (
来源：http://hz.0kj1m.cn/gtieedtbsb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.quarkkingdee.top/gtpydtunyd.html

) t WHERE rn = 1;
来源：http://hz.zhongyouzk.top/gtkfytqhwq.html

[Q35] 内连接
来源：http://hz.yongpay.top/gtwvmyojap.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jlsjyb.cn/gtvhdtzqlm.html

[Q36] 左连接
来源：http://hz.c1oappe.top/gtdffqgoor.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.snrcjt.cn/gtjkzvyzzf.html

[Q37] 右连接
来源：http://hz.daxiang520.top/gtnykknhpr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hysaishi.cn/gtxwapkuxf.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangdashe.top/gtjvtgmurs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.daxiang520.top/gtrcftmhix.html

[Q39] 自连接（查上下级）
来源：http://hz.zhengqikj.top/gtqjxoqtmc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.daxiang520.top/gtrrlozwhp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.0kj1m.cn/gtsymtowmm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.wangdashe.top/gtjegjhidx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hysaishi.cn/gtvazdlhyc.html

[Q41] 多表连接
来源：http://hz.cqqwz.cn/gtlnidpbtb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.feifeiyinyue.top/gtltfkybcu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.tanke756.top/gtydgvujfa.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.snrcjt.cn/gtantbluxw.html

[Q42] 连接条件附加过滤
来源：http://hz.fengsongda.top/gtwaxmuuoy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sxryk.cn/gtferqabhp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.tianlin.xyz/gtksuebpbv.html

[Q43] 标量子查询
来源：http://hz.sysykeji.top/gtlwfkmpyv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jianghu66.top/gtzstcrzpt.html

[Q44] IN 子查询
来源：http://hz.shanyushiyangtech.top/gtpalrxrlw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cheryme.top/gtjzorlsje.html

[Q45] EXISTS 判断存在
来源：http://hz.mhx1999.top/gtmpxnyjxc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangshuangyany.cn/gtdwwxlztq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xuetiantiany.cn/gtdkotzxfm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhiwuduotai.top/gtjeynzhpg.html

[Q47] 与平均值比较
来源：http://hz.mhx1999.top/gteugrjolm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shzxlz.cn/gtxwtabdhg.html

[Q48] CTE 公用表表达式
来源：http://hz.c1oappe.top/gttezybjqc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yangfankeji.com/gtfljclrxh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xinyue.icu/gtonftfrzs.html

[Q49] 更新单行
来源：http://hz.hywenlv.cn/gtyglhtzce.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhiwuduotai.top/gtkgdmslcq.html

[Q50] 批量更新
来源：http://hz.shangyingyoupin.top/gtvoywusri.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gzhubu.top/gtyyknnyqw.html

[Q51] 用子查询更新
来源：http://hz.vqdsnc.cn/gtdffdedpq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yongpay.top/gtyfarfxvw.html

[Q52] 删除指定行
来源：http://hz.shzxlz.cn/gtjqgrccqc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hnxiangtu.top/gtzdkrertt.html

[Q53] 按条件删除
来源：http://hz.xuanzx.com/gtdmcptlkp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhengqikj.top/gtwiqqphpm.html

[Q54] 清空表
来源：http://hz.tanke756.top/gtjehznunw.html

TRUNCATE TABLE logs;
来源：http://hz.xuanzx.com/gtxuimllyi.html

[Q55] 排名（并列占位）
来源：http://hz.haohaochexian.top/gtbcijlals.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jiagoushi.top/gtbanghqka.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zdqjudy.top/gtwyswhgaa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.52xcode.cn/gtdqqjvpuc.html

[Q57] 行号
来源：http://hz.smart0.xyz/gtpbjxwbwt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cucudq.cn/gtecrkwaoe.html

[Q58] 累计求和
来源：http://hz.jinyuanbaomall.cn/gteliowpnd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ivvv.top/gtsrpeordg.html

[Q59] 分组内累计
来源：http://hz.jyoumei.cn/gtgdgxyjvx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtyapuxmdj.html

[Q60] 取上一行 / 下一行
来源：http://hz.jinyuanbaomall.cn/gtgywbxaom.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj20258.top/gtfykogwnn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.wangdashe.top/gtaljnoido.html

[Q61] 移动平均
来源：http://hz.zhiwuduotai.top/gtqgjoqsbg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.pengpengdd.cyou/gtypwpkwup.html

[Q62] 分组占比
来源：http://hz.jinyuanbaomall.cn/gtbqmuldtt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gtrpptienn.html

[Q63] 开启事务
来源：http://hz.cdnleiting.top/gtroooudts.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hnqzz.top/gtwtwuuhzk.html

[Q64] 提交事务
来源：http://hz.iojbl.cn/gtcvhtzoxv.html

COMMIT;
来源：http://hz.fengsongda.top/gtixuticwi.html

[Q65] 回滚事务
来源：http://hz.shzxlz.cn/gtnomxbngt.html

ROLLBACK;
来源：http://hz.jlsjyb.cn/gteblcaufd.html

[Q66] 行锁查询
来源：http://hz.nanxuanxn.top/gtihxlsxho.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yongpay.top/gtpozknjmv.html

[Q67] 设置隔离级别
来源：http://hz.c1oappe.top/gtjckxkdxx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.guowangkeji.top/gtejiohktt.html

[Q68] 保存点
来源：http://hz.shanyushiyangtech.top/gtmdvrhpgh.html

SAVEPOINT sp1;
来源：http://hz.smart0.xyz/gtfezyjojn.html

ROLLBACK TO sp1;
来源：http://hz.ydzc1.top/gtytwvigbz.html

[Q69] 查看执行计划
来源：http://hz.fengsongda.top/gtosbbzbep.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gotoacloud.top/gthaerbhfc.html

[Q70] 更新统计信息
来源：http://hz.jqgfzy.top/gtwvefdyok.html

ANALYZE TABLE users;
来源：http://hz.ydjk.org.cn/gthfmxxixx.html

[Q71] 查看建表语句
来源：http://hz.xuetiantiany.cn/gttzowvebi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.wangdashe.top/gtoppimiyi.html

[Q72] 查看索引
来源：http://hz.xylfe.cn/gtsvnzpwew.html

SHOW INDEX FROM users;
来源：http://hz.ydjk.org.cn/gtvprbiwxi.html

[Q73] 查看表状态
来源：http://hz.wangshuangyany.cn/gttfuajcng.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ehwqpu.com/gtnzsuoprd.html

[Q74] 强制使用索引
来源：http://hz.vqdsnc.cn/gthawnabwc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.vqdsnc.cn/gtjbvesbxv.html

[Q75] 日期格式化
来源：http://hz.yj20258.top/gturqwhkbq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cashguo.top/gtnkglmaur.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.tianlin.xyz/gtxscmprbw.html

[Q76] 按天统计
来源：http://hz.xinyue.icu/gtfssobgaj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.guowangkeji.top/gtjocnmzhx.html

[Q77] 时间加减
来源：http://hz.andypj.xyz/gtpuezcaur.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cheryme.top/gtpqfokpap.html

[Q78] 当前时间
来源：http://hz.gotoacloud.top/gtgszumxbb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.tanke756.top/gtzfsjismx.html

[Q79] 字符串拼接
来源：http://hz.guannengcc.top/gtiykystts.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sweek.top/gtgntpkyfy.html

[Q80] 字符串截取
来源：http://hz.jlsjyb.cn/gtnintisoj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinqigufen.top/gtaksryxey.html

[Q81] 字符串替换
来源：http://hz.ppjwa.cn/gtanbckbms.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jqgfzy.top/gttcldnont.html

[Q82] 字符长度与字节长度
来源：http://hz.tianlin.xyz/gtuzjgarya.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinqigfzy.top/gtsktvlsjw.html

[Q83] 大小写转换
来源：http://hz.cashguo.top/gtpcuilggy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.smart0.xyz/gttxpciogo.html

[Q84] 去除首尾空格
来源：http://hz.ehwqpu.com/gtbtunduxx.html

SELECT TRIM(name) FROM users;
来源：http://hz.xziqi.cn/gtyvsdbyro.html

[Q85] 数值取整
来源：http://hz.ydjk.org.cn/gtkftvjgef.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.iojbl.cn/gtxnwibudn.html

[Q86] 读取 JSON 字段
来源：http://hz.shzxlz.cn/gtlwrnerbv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cashguo.top/gtjtziqutg.html

[Q87] JSON 字段做条件
来源：http://hz.sufxvd.cn/gtbrbxieke.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.redwolf501.top/gtpngbfzef.html

[Q88] 行转列（条件聚合）
来源：http://hz.tianlin.xyz/gtynhsylwk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.kuanghao11.cn/gtglulyfko.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gotoacloud.top/gtosfcjgwy.html

[Q89] 判断表是否存在
来源：http://hz.hnqzz.top/gtgfvntzzo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhengqikj.top/gtvgfawxps.html

[Q90] 生成序号列
来源：http://hz.kuanghao11.cn/gtwpizoohe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.feifeiyinyue.top/gthghrbwym.html

================================================================================
来源：http://hz.hammf.cn/gtzjkituoa.html

R. Bash 专题
来源：http://hz.iojbl.cn/gtnfedisdb.html

================================================================================
来源：http://hz.smart0.xyz/gtsjjlfque.html

[R01] shebang 与严格模式
来源：http://hz.fengsongda.top/gtryeaihkh.html

#!/usr/bin/env bash
来源：http://hz.jlsjyb.cn/gtuxyljmad.html

set -euo pipefail
来源：http://hz.316326.xyz/gtwdwtmynh.html

[R02] 变量赋值与使用
来源：http://hz.hywenlv.cn/gtecymfmhm.html

name="Tom"; echo "$name"
来源：http://hz.52xcode.cn/gtwkvhxafh.html

[R03] 只读变量
来源：http://hz.jqgfzy.top/gtmtrwgyzn.html

readonly PI=3.14
来源：http://hz.haohaochexian.top/gtxyajibun.html

[R04] 位置参数
来源：http://hz.316326.xyz/gtoxjxcqsl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhongyouzk.top/gtoqfxerhr.html

[R05] 参数默认值
来源：http://hz.jqgfzy.top/gtymutorwl.html

name="${1:-default}"
来源：http://hz.vqdsnc.cn/gtuhwppoqq.html

[R06] 判断命令是否存在
来源：http://hz.jianghu66.top/gtjyjcvhfc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhoulong.xyz/gtkiftxgpm.html

[R07] if 判断文件
来源：http://hz.pengpengdd.cyou/gtdlvvzwla.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guannengcc.top/gtwvekuawx.html

[R08] 数值比较
来源：http://hz.cheryme.top/gtflfhsiwb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinqigufen.top/gtdkidmris.html

[R09] 字符串比较
来源：http://hz.jinqigfzy.top/gtxzhjqhes.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.nanxinkj.top/gtvrizfydw.html

[R10] 正则匹配
来源：http://hz.zdqjudy.top/gtqlztpvio.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jianghu66.top/gtldrusjwf.html

[R11] case 多分支
来源：http://hz.ehwqpu.com/gtaeddocim.html

case "$1" in
来源：http://hz.jianghu66.top/gtmlwhlhyl.html

start) echo "启动" ;;
来源：http://hz.iojbl.cn/gtkmgcxpfl.html

stop)  echo "停止" ;;
来源：http://hz.zhengqikj.top/gtfsfncpil.html

*)     echo "未知命令" ;;
来源：http://hz.mhx1999.top/gtxitszshq.html

esac
来源：http://hz.dashuyun.cn/gtmpdmqndy.html

[R12] for 遍历文件
来源：http://hz.jinghuilouyu.cn/gtoyukawhl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.daria6918.cn/gtxonmylxw.html

[R13] for 计数循环
来源：http://hz.xingfuxueyuan.xyz/gtuwjxtgsl.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.vqdsnc.cn/gtxafwrkpm.html

[R14] C 风格 for
来源：http://hz.ywan-chungtsiang.top/gtnylsasxe.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.guowangkeji.top/gtfgojerqi.html

[R15] while 逐行读文件
来源：http://hz.quarkkingdee.top/gthzvkdodh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sxryk.cn/gtordsiowx.html

[R16] until 等待条件
来源：http://hz.xuetiantiany.cn/gthuslhntb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.fzhhl.top/gtjzfwbdrw.html

[R17] 数组定义与取值
来源：http://hz.yuanzhike.top/gtwbirptfu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.pengpengdd.cyou/gtazrsplcv.html

[R18] 遍历数组
来源：http://hz.xuanzx.com/gtrlaxyzyb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.aizwys.cn/gttkkgwbhi.html

[R19] 数组长度
来源：http://hz.yueranfly.top/gtdbuovcmb.html

echo "${#arr[@]}"
来源：http://hz.tian-w.cn/gtvmfafthf.html

[R20] 关联数组（字典）
来源：http://hz.yj20258.top/gtbddxkchq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.birdmap.top/gtqffrtwlm.html

[R21] 字符串长度
来源：http://hz.haohaochexian.top/gtmdplfszh.html

echo "${#s}"
来源：http://hz.xingfuxueyuan.xyz/gteujebrmn.html

[R22] 截取子串
来源：http://hz.hywenlv.cn/gtcvfrayfs.html

echo "${s:0:5}"
来源：http://hz.wangdashe.top/gtfjftqwgn.html

[R23] 字符串替换
来源：http://hz.yj20258.top/gtjamoxkge.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.tianlin.xyz/gtwswrgtui.html

[R24] 大小写转换
来源：http://hz.redwolf501.top/gthdnrmpwq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.316326.xyz/gttdizhcbd.html

[R25] 去后缀 / 去前缀
来源：http://hz.pycfn.com/gtfnianonl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yvedp.cn/gtefmbrutx.html

[R26] 命令替换
来源：http://hz.chenjidiqi.icu/gtkzbpalxu.html

now=$(date +%F); echo "$now"
来源：http://hz.0kj1m.cn/gtrqutpfhp.html

[R27] 算术展开
来源：http://hz.fzhhl.top/gtdfykzrds.html

echo $((1 + 2 * 3))
来源：http://hz.hammf.cn/gtjvezhauw.html

[R28] 浮点运算
来源：http://hz.cashguo.top/gtakakiqhb.html

echo "scale=2; 10/3" | bc
来源：http://hz.yanxiufei.cn/gtyatauyue.html

[R29] 定义函数
来源：http://hz.havefunace.top/gtvjdcdqnr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xziqi.cn/gtpsiluefn.html

[R30] 函数返回状态码
来源：http://hz.ivvv.top/gtagovuuej.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yueranfly.top/gtylnpvweg.html

[R31] 局部变量
来源：http://hz.zhiwuduotai.top/gthyoaecgl.html

f() { local x=1; echo "$x"; }
来源：http://hz.sysykeji.top/gtlmjgaqqi.html

[R32] 参数个数校验
来源：http://hz.sxryk.cn/gtkmxhvqgy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yongpay.top/gtzmalnflr.html

[R33] 捕获错误并提示行号
来源：http://hz.aibaodan.cn/gttitqigdo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jyoumei.cn/gtjikfrxzg.html

[R34] 退出时清理
来源：http://hz.shanyushiyangtech.top/gtcspymdsi.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258888.top/gtnmccnfzl.html

[R35] 后台执行并等待
来源：http://hz.zhijiandao.cn/gtgkghvwhq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.fengsongda.top/gtwnncoahf.html

[R36] 并发执行多个任务
来源：http://hz.cqqwz.cn/gtfzlgxmjm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinyuanbaomall.cn/gtzfwcrzmm.html

[R37] 把输出赋给变量
来源：http://hz.chenjidiqi.icu/gtgjppaztd.html

files=$(ls -1)
来源：http://hz.hfpthk.cn/gtbspdehgd.html

[R38] 管道串联
来源：http://hz.hysaishi.cn/gtgxvnntzn.html

cat a.txt | grep -i error | wc -l
来源：http://hz.guannengcc.top/gthgvvifyq.html

[R39] 重定向标准输出与错误
来源：http://hz.daxiang520.top/gtwqqhzevw.html

cmd > out.log 2>&1
来源：http://hz.hfpthk.cn/gtrzkzhsyn.html

[R40] 追加写日志
来源：http://hz.316326.xyz/gtjablazhn.html

echo "log" >> out.log
来源：http://hz.zhoulong.xyz/gtqhkfavuk.html

[R41] 丢弃输出
来源：http://hz.gzhubu.top/gtmfntokbk.html

cmd >/dev/null 2>&1
来源：http://hz.birdmap.top/gtovpspxnv.html

[R42] 输入重定向
来源：http://hz.c1oappe.top/gtgebrijkz.html

wc -l < a.txt
来源：http://hz.pengpengdd.cyou/gtdnxulifs.html

[R43] 按名字查找文件
来源：http://hz.guannengcc.top/gtcakygmzm.html

find . -name "*.log" -type f
来源：http://hz.wangdashe.top/gthaadetcq.html

[R44] 按修改时间查找
来源：http://hz.yonumen.top/gtdlijmqdz.html

find . -mtime -7 -type f
来源：http://hz.jinyuanbaomall.cn/gtjajibyqf.html

[R45] 批量删除
来源：http://hz.gogol.net.cn/gtxylxpgjn.html

find . -name "*.tmp" -delete
来源：http://hz.wangdashe.top/gtzlrdbswa.html

[R46] 递归替换文件内容
来源：http://hz.shuidangran.top/gteaofaypm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yvedp.cn/gtjogbhkip.html

[R47] sed 单行替换
来源：http://hz.zhixingplan.top/gtccqzezhe.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.pengpengdd.cyou/gtesfdjaem.html

[R48] awk 取指定列
来源：http://hz.cheryme.top/gtkwueabie.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj20258.top/gtxwdinrjg.html

[R49] awk 带条件
来源：http://hz.zhaomingkeji.xyz/gtdnlvowkv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jyoumei.cn/gtemupqeds.html

[R50] awk 求和
来源：http://hz.havefunace.top/gtplyqfriz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xuanzx.com/gtmirtnqtm.html

[R51] 排序去重取前几
来源：http://hz.shanyushiyangkeji.top/gtciyjkcyf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.fengsongda.top/gtvyqafrkf.html

[R52] 统计行数
来源：http://hz.yuxming.cn/gthotgppsb.html

wc -l a.txt
来源：http://hz.hnqzz.top/gtmimvpqfi.html

[R53] 查看文件头与实时尾
来源：http://hz.ybcxt.top/gtedelrlal.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.tian-w.cn/gtgpxosfau.html

[R54] 比较两个文件
来源：http://hz.dianchejie.cn/gtfbmbsjcz.html

diff a.txt b.txt
来源：http://hz.ehwqpu.com/gtsjmepimn.html

[R55] 压缩与解压
来源：http://hz.cashguo.top/gtdxraxllp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhijiandao.cn/gtjolaghae.html

[R56] 远程拷贝
来源：http://hz.ydzc1.top/gtrqaybtnj.html

scp file user@host:/path/
来源：http://hz.vqdsnc.cn/gtwxcleycz.html

[R57] 远程执行命令
来源：http://hz.tanke756.top/gtgehwfjrk.html

ssh user@host 'uptime'
来源：http://hz.dianchejie.cn/gtxsfwprsq.html

[R58] 下载文件
来源：http://hz.zdqjudy.top/gtemgwsitf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhengqikj.top/gtqoujkgha.html

[R59] 发 POST JSON
来源：http://hz.jyoumei.cn/gtflbqjynu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.iojbl.cn/gtczykunwp.html

[R60] 只看 HTTP 状态码
来源：http://hz.iojbl.cn/gtjprdgjgy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xuanzx.com/gtoynnvjwb.html

[R61] 磁盘占用
来源：http://hz.cqqwz.cn/gteucuhswe.html

df -h;  du -sh *
来源：http://hz.ehwqpu.com/gtfsesokiv.html

[R62] 找最占空间的文件
来源：http://hz.hongshengwenyu.top/gtytquyies.html

du -ah . | sort -rh | head -10
来源：http://hz.zhixingplan.top/gtbzwboexe.html

[R63] 内存与进程
来源：http://hz.daria6918.cn/gtfhaudrlq.html

free -h;  ps aux | grep nginx
来源：http://hz.andypj.xyz/gtqlmucssc.html

[R64] 结束进程
来源：http://hz.dianchejie.cn/gtqwvkhcty.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yueranfly.top/gtelxovyae.html

[R65] 查看端口占用
来源：http://hz.c1oappe.top/gtpvtugrmg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sxryk.cn/gtqgspobcw.html

[R66] 定时任务
来源：http://hz.sysykeji.top/gtizjisjem.html

crontab -e;  crontab -l
来源：http://hz.meibo888.top/gtbwmnxrrv.html

[R67] 生成随机十六进制串
来源：http://hz.vqdsnc.cn/gtiycghdyw.html

openssl rand -hex 16
来源：http://hz.cheryme.top/gtxjlgvomh.html

[R68] 计算文件校验值
来源：http://hz.xziqi.cn/gtdrprqitu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.fzhhl.top/gtkvwjvbaa.html

[R69] 生成随机密码
来源：http://hz.pengpengdd.cyou/gtlsojssok.html

head -c 16 /dev/urandom | base64
来源：http://hz.xziqi.cn/gtjgegexex.html

[R70] 时间戳与互转
来源：http://hz.zhijiandao.cn/gttedhyglb.html

date +%s;  date -d @1700000000
来源：http://hz.daria6918.cn/gthdzporrq.html

[R71] 日期格式化
来源：http://hz.jyoumei.cn/gtcvmkgidh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ybcxt.top/gtnpnjgbce.html

[R72] 等待端口就绪
来源：http://hz.mhx1999.top/gtcbklltsj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sweek.top/gtvvdkuvmp.html

[R73] 分割大日志
来源：http://hz.chenjidiqi.icu/gtrlrkihjg.html

split -l 1000 big.log part_
来源：http://hz.yonumen.top/gtmzrjfjpr.html

[R74] 批量重命名
来源：http://hz.ydjk.org.cn/gtdhgalwpj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hysaishi.cn/gttplqvyli.html

[R75] 导出环境变量
来源：http://hz.dianchejie.cn/gtsizlzsir.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yangfankeji.com/gtyjiohrbr.html

[R76] 使用临时文件
来源：http://hz.jiagoushi.top/gtsvkzvsup.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.aizwys.cn/gtyqavftfj.html

[R77] 读取用户输入
来源：http://hz.chenlongwang.top/gtghlwgsvw.html

read -rp "请输入: " ans
来源：http://hz.ydjk.org.cn/gtxgrwlqgy.html

[R78] 交互式菜单
来源：http://hz.chenzaomai.com/gtlggsqyrk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.redwolf501.top/gtlrqbphwz.html

[R79] 解析命令行选项
来源：http://hz.havefunace.top/gtpvdhyale.html


<!-- 参考信息 -->