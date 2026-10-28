代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ydjk.org.cn/gtwuftadst.html

[Q20] IN 列表
来源：http://hz.jyoumei.cn/gthirtntmt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jiagoushi.top/gttuwtgnoj.html

[Q21] 空值判断
来源：http://hz.zycfv.cn/gtzadrqion.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.bjfxy.top/gtgsqjtgvg.html

[Q22] 排序
来源：http://hz.yvedp.cn/gtaiqklzkh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tian-w.cn/gtjugeassx.html

[Q23] 分页
来源：http://hz.svipenyu.cn/gthsxwpofq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.havefunace.top/gteanyrvhj.html

[Q24] 去重
来源：http://hz.zhijiandao.cn/gtlpheqyyz.html

SELECT DISTINCT city FROM users;
来源：http://hz.9152youxi.cn/gtfnqwyuag.html

[Q25] 只取前 N 条
来源：http://hz.yvedp.cn/gtqrpnsmdw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.tanke756.top/gtbuccgfxc.html

[Q26] 计数
来源：http://hz.vqdsnc.cn/gtlcmmzqar.html

SELECT COUNT(*) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtupnhnuip.html

[Q27] 条件计数
来源：http://hz.bjfxy.top/gtdvyqjfsa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yanxiufei.cn/gtbvpfxhje.html

[Q28] 求和与平均
来源：http://hz.redwolf501.top/gtdoofpbsu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtsgnblbyx.html

[Q29] 最大最小值
来源：http://hz.52xcode.cn/gtgqasnodu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.aibaodan.cn/gtylqvjatp.html

[Q30] 分组统计
来源：http://hz.cheryme.top/gtlvuabprp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtqmbtcryh.html

[Q31] 分组后过滤
来源：http://hz.snrcjt.cn/gtcfnsgmay.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.c1oappe.top/gtvthgnaam.html

[Q32] 分组拼接字符串
来源：http://hz.yj202588.top/gtdqcnsewo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.guannengcc.top/gtlyjvdsqw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gotoacloud.top/gtzjanifwz.html

[Q33] 多列分组
来源：http://hz.pengpengdd.cyou/gtgypqbute.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tianlin.xyz/gtscmqpcjs.html

[Q34] 每组取第一条
来源：http://hz.cashguo.top/gtrsbtdlrj.html

SELECT * FROM (
来源：http://hz.sysykeji.top/gtahxdlvbo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ppjwa.cn/gtclchnfyc.html

) t WHERE rn = 1;
来源：http://hz.meibo888.top/gtzfmokkzw.html

[Q35] 内连接
来源：http://hz.cheryme.top/gtmviwhosa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cqqwz.cn/gtyoltbdvk.html

[Q36] 左连接
来源：http://hz.feifeiyinyue.top/gtcuiolohp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydzc1.top/gtptuoddzw.html

[Q37] 右连接
来源：http://hz.smart0.xyz/gtqbcogbxv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.iojbl.cn/gttxcehdum.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yongpay.top/gtrgcehvot.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shanyushiyangtech.top/gteypvkjvq.html

[Q39] 自连接（查上下级）
来源：http://hz.hywenlv.cn/gtnbodehge.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.guannengcc.top/gttmkbwbwy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.pycfn.com/gtzpzeivjb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.316326.xyz/gttycyalex.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sysykeji.top/gtffxgijbe.html

[Q41] 多表连接
来源：http://hz.cheryme.top/gtktocizqt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.meibo888.top/gtofdcevsv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.nwbrower.top/gtvdbjrbvb.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gogol.net.cn/gtbkijdijr.html

[Q42] 连接条件附加过滤
来源：http://hz.shzxlz.cn/gtgsafzngh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.vqdsnc.cn/gtuypjbxkd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jyoumei.cn/gtbzyoxscr.html

[Q43] 标量子查询
来源：http://hz.tanke756.top/gtyplwudwu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.tanke756.top/gtyqvobodi.html

[Q44] IN 子查询
来源：http://hz.xylfe.cn/gtrkyufezh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cdnleiting.top/gtzaqmyyds.html

[Q45] EXISTS 判断存在
来源：http://hz.yonumen.top/gtwwkjwrsf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tianlin.xyz/gtzhdfalrh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sysykeji.top/gtbusrjzhg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangdashe.top/gtmsvrjbhy.html

[Q47] 与平均值比较
来源：http://hz.shangyingyoupin.top/gtnzglkxca.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhixingplan.top/gtvafajdep.html

[Q48] CTE 公用表表达式
来源：http://hz.hysaishi.cn/gtavhhmwty.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gaohongyu789.top/gteicidkhi.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tian-w.cn/gtgiqknlsn.html

[Q49] 更新单行
来源：http://hz.tanke756.top/gtvmgldorf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xinyue.icu/gtgcaciczy.html

[Q50] 批量更新
来源：http://hz.tanke756.top/gtuqmmizcp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yangfankeji.com/gtkonxzglj.html

[Q51] 用子查询更新
来源：http://hz.tianlin.xyz/gtcvkudjcf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hywenlv.cn/gtiowztkis.html

[Q52] 删除指定行
来源：http://hz.mhx1999.top/gtgllchmdq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.dianchejie.cn/gtygkigtjq.html

[Q53] 按条件删除
来源：http://hz.aibaodan.cn/gtitszubrt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yuanzhike.top/gtwglisyqv.html

[Q54] 清空表
来源：http://hz.xylfe.cn/gtburqrzwo.html

TRUNCATE TABLE logs;
来源：http://hz.jlsjyb.cn/gtqragndhk.html

[Q55] 排名（并列占位）
来源：http://hz.sxryk.cn/gtiztiqrgs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cqqwz.cn/gtaqdldkbe.html

[Q56] 密集排名（并列不占位）
来源：http://hz.tanke756.top/gtgaagvyak.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.aibaodan.cn/gtiuaeepqc.html

[Q57] 行号
来源：http://hz.dianchejie.cn/gtapolztca.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yuxming.cn/gtwpcjrgtz.html

[Q58] 累计求和
来源：http://hz.ybcxt.top/gtjxjjfmvn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cqqwz.cn/gtolinytwc.html

[Q59] 分组内累计
来源：http://hz.meibo888.top/gtnorznfyl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yonumen.top/gtpeuagixo.html

[Q60] 取上一行 / 下一行
来源：http://hz.xinyue.icu/gtemxrhgcc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.316326.xyz/gtfyijipbm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenlongwang.top/gtdqskgfkp.html

[Q61] 移动平均
来源：http://hz.yj20258888.top/gtnilqjbmp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.aibaodan.cn/gturohilwf.html

[Q62] 分组占比
来源：http://hz.zhiwuduotai.top/gtqivmlxlc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hnxiangtu.top/gtyaocsydj.html

[Q63] 开启事务
来源：http://hz.zhixingplan.top/gtrtnuiaya.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sysykeji.top/gtsuyiiytx.html

[Q64] 提交事务
来源：http://hz.yuanzhike.top/gtxznpdmtz.html

COMMIT;
来源：http://hz.zhijiandao.cn/gtvxawanbi.html

[Q65] 回滚事务
来源：http://hz.zdqjudy.top/gtehqrvttt.html

ROLLBACK;
来源：http://hz.ybcxt.top/gtzizbnqpo.html

[Q66] 行锁查询
来源：http://hz.nanxuanxn.top/gtguedjydv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hfpthk.cn/gtsykxgvsp.html

[Q67] 设置隔离级别
来源：http://hz.zhixingplan.top/gtnsvpgyrw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gaohongyu789.top/gtewmbqbbp.html

[Q68] 保存点
来源：http://hz.aizwys.cn/gtnfvaaqrc.html

SAVEPOINT sp1;
来源：http://hz.sufxvd.cn/gturtcalfw.html

ROLLBACK TO sp1;
来源：http://hz.tian-w.cn/gtyrhqghdt.html

[Q69] 查看执行计划
来源：http://hz.ppjwa.cn/gtipxunkgi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shuidangran.top/gthfiowgns.html

[Q70] 更新统计信息
来源：http://hz.jinqigufen.top/gtadiluyxy.html

ANALYZE TABLE users;
来源：http://hz.yonumen.top/gthoiwxloa.html

[Q71] 查看建表语句
来源：http://hz.hfpthk.cn/gtkcmsrbji.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sxryk.cn/gtefbfditg.html

[Q72] 查看索引
来源：http://hz.ivvv.top/gtiezopjyx.html

SHOW INDEX FROM users;
来源：http://hz.snrcjt.cn/gtoeonneqy.html

[Q73] 查看表状态
来源：http://hz.yuanzhike.top/gtqekakkoq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.tian-w.cn/gtgrimgdyh.html

[Q74] 强制使用索引
来源：http://hz.ppjwa.cn/gtmbrunvvi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.iojbl.cn/gtubvrhnci.html

[Q75] 日期格式化
来源：http://hz.nanxuanxn.top/gtbglwzwke.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.fzhhl.top/gtjqvtezij.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nanxinkj.top/gtlqypzers.html

[Q76] 按天统计
来源：http://hz.svipenyu.cn/gtlhjyldyd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xuetiantiany.cn/gtgojlsocy.html

[Q77] 时间加减
来源：http://hz.iojbl.cn/gtnvqtpgct.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.iojbl.cn/gtkfxhmngm.html

[Q78] 当前时间
来源：http://hz.hnxiangtu.top/gtinmtkyqn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.wangshuangyany.cn/gterkiczdw.html

[Q79] 字符串拼接
来源：http://hz.ivvv.top/gtyowigqjx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinqigufen.top/gtvhrwlgcw.html

[Q80] 字符串截取
来源：http://hz.dianchejie.cn/gtncnigogp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xuetiantiany.cn/gtwzmgkaam.html

[Q81] 字符串替换
来源：http://hz.xuanzx.com/gtybjyrwab.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.9152youxi.cn/gtyfhejorg.html

[Q82] 字符长度与字节长度
来源：http://hz.zhijiandao.cn/gtydqotkbv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hywenlv.cn/gtqnicijlr.html

[Q83] 大小写转换
来源：http://hz.haohaochexian.top/gthjjhagkm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yuxming.cn/gtrpkkphct.html

[Q84] 去除首尾空格
来源：http://hz.yongpay.top/gthxmesowo.html

SELECT TRIM(name) FROM users;
来源：http://hz.dianchejie.cn/gtbeojycgi.html

[Q85] 数值取整
来源：http://hz.yuxming.cn/gtztmsouet.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jiagoushi.top/gtmhrirdly.html

[Q86] 读取 JSON 字段
来源：http://hz.xuetiantiany.cn/gtpadpieid.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cdnleiting.top/gtddhgwtrk.html

[Q87] JSON 字段做条件
来源：http://hz.ywan-chungtsiang.top/gtqucbydok.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xuanzx.com/gtqasqlaho.html

[Q88] 行转列（条件聚合）
来源：http://hz.hywenlv.cn/gtpinxaspj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.havefunace.top/gtrukulgfe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ybcxt.top/gtercqhmhx.html

[Q89] 判断表是否存在
来源：http://hz.snrcjt.cn/gtzudyvohd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hysaishi.cn/gtrqskuttg.html

[Q90] 生成序号列
来源：http://hz.jinghuilouyu.cn/gtddppprby.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinyuanbaomall.cn/gtjineulhv.html

================================================================================
来源：http://hz.yj20258.top/gtrupeghvn.html

R. Bash 专题
来源：http://hz.yangfankeji.com/gtajesodkh.html

================================================================================
来源：http://hz.jianghu66.top/gtgameclwa.html

[R01] shebang 与严格模式
来源：http://hz.ivvv.top/gtezkxmqnt.html

#!/usr/bin/env bash
来源：http://hz.ybcxt.top/gtnquflutm.html

set -euo pipefail
来源：http://hz.dianchejie.cn/gtqvidwkcl.html

[R02] 变量赋值与使用
来源：http://hz.nanxinkj.top/gtnrsnrkcy.html

name="Tom"; echo "$name"
来源：http://hz.hnqzz.top/gtzyyxncpf.html

[R03] 只读变量
来源：http://hz.yueranfly.top/gtbofsuxrn.html

readonly PI=3.14
来源：http://hz.zhaomingkeji.xyz/gtxmbcrnzd.html

[R04] 位置参数
来源：http://hz.wangdashe.top/gthsiercxa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenjidiqi.icu/gtjabzakkr.html

[R05] 参数默认值
来源：http://hz.zhaomingkeji.xyz/gtgbonnhcz.html

name="${1:-default}"
来源：http://hz.shzxlz.cn/gtvjveaouz.html

[R06] 判断命令是否存在
来源：http://hz.fzhhl.top/gtojzbjuso.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shuidangran.top/gteapajqeg.html

[R07] if 判断文件
来源：http://hz.jinghuilouyu.cn/gthpgkmfom.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.havefunace.top/gtidjmadnd.html

[R08] 数值比较
来源：http://hz.pycfn.com/gtgrmlvtjk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jiagoushi.top/gtolchojtf.html

[R09] 字符串比较
来源：http://hz.jianghu66.top/gtxmabxjrs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.andypj.xyz/gtzgcuujlo.html

[R10] 正则匹配
来源：http://hz.bjfxy.top/gtrgocwtsw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinqigufen.top/gtzbfvwtkv.html

[R11] case 多分支
来源：http://hz.yj202588.top/gtoootekze.html

case "$1" in
来源：http://hz.wangshuangyany.cn/gtxwmglivc.html

start) echo "启动" ;;
来源：http://hz.chenlongwang.top/gtahsgmorp.html

stop)  echo "停止" ;;
来源：http://hz.jlsjyb.cn/gtxjwfwmua.html

*)     echo "未知命令" ;;
来源：http://hz.ivvv.top/gtlubhiqey.html

esac
来源：http://hz.c1oappe.top/gtorjrgzvs.html

[R12] for 遍历文件
来源：http://hz.dashuyun.cn/gthidpkeel.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ydjk.org.cn/gttavwmunj.html

[R13] for 计数循环
来源：http://hz.ivvv.top/gtjdsyfpfb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinqigfzy.top/gtmmzwkmfs.html

[R14] C 风格 for
来源：http://hz.jqgfzy.top/gtqyalkwus.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jyoumei.cn/gtslflcyqq.html

[R15] while 逐行读文件
来源：http://hz.jyoumei.cn/gtvtgeuegs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.vqdsnc.cn/gtgvunplgw.html

[R16] until 等待条件
来源：http://hz.nanxinkj.top/gtcyetztxr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yueranfly.top/gtishdqgyx.html

[R17] 数组定义与取值
来源：http://hz.xinyue.icu/gtwaaplmit.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ywan-chungtsiang.top/gtyanofdxc.html

[R18] 遍历数组
来源：http://hz.zhiwuduotai.top/gtkmpochox.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gzhubu.top/gtffyxgidg.html

[R19] 数组长度
来源：http://hz.zhoulong.xyz/gtxlzcdhfc.html

echo "${#arr[@]}"
来源：http://hz.tanke756.top/gtwgytgjdh.html

[R20] 关联数组（字典）
来源：http://hz.fzhhl.top/gtmcmuotkc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gogol.net.cn/gtgryumfie.html

[R21] 字符串长度
来源：http://hz.ydzc1.top/gtzgtvuuic.html

echo "${#s}"
来源：http://hz.yvedp.cn/gtnwtprotf.html

[R22] 截取子串
来源：http://hz.yonumen.top/gtthharbri.html

echo "${s:0:5}"
来源：http://hz.ppjwa.cn/gtltgnscze.html

[R23] 字符串替换
来源：http://hz.haohaochexian.top/gtdkohvkyl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xuetiantiany.cn/gtkreujneq.html

[R24] 大小写转换
来源：http://hz.wangdashe.top/gtqljxecwg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.mhx1999.top/gtwzswseyw.html

[R25] 去后缀 / 去前缀
来源：http://hz.shangyingyoupin.top/gtchsfipab.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.tianlin.xyz/gtxvvkvuge.html

[R26] 命令替换
来源：http://hz.sweek.top/gthwankkjd.html

now=$(date +%F); echo "$now"
来源：http://hz.zhoulong.xyz/gtatmgpxqs.html

[R27] 算术展开
来源：http://hz.cdnleiting.top/gtiberksyl.html

echo $((1 + 2 * 3))
来源：http://hz.jlsjyb.cn/gtgwpfqequ.html

[R28] 浮点运算
来源：http://hz.jianghu66.top/gttsyhmivb.html

echo "scale=2; 10/3" | bc
来源：http://hz.gaohongyu789.top/gtnjaeqszv.html

[R29] 定义函数
来源：http://hz.chenlongwang.top/gtitjgdekj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj20258888.top/gthxhfqbiv.html

[R30] 函数返回状态码
来源：http://hz.chenjidiqi.icu/gtapzdebsb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jiagoushi.top/gtzpfyqpgy.html

[R31] 局部变量
来源：http://hz.zhoulong.xyz/gtrhenfhmi.html

f() { local x=1; echo "$x"; }
来源：http://hz.feifeiyinyue.top/gtcuqniqjz.html

[R32] 参数个数校验
来源：http://hz.redwolf501.top/gtodiotvvk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cheryme.top/gtholuvrbr.html

[R33] 捕获错误并提示行号
来源：http://hz.nanxinkj.top/gtyhnxrtag.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj202588.top/gtsbeqpnvp.html

[R34] 退出时清理
来源：http://hz.bjfxy.top/gtwmzszdvu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtfbyvjqoe.html

[R35] 后台执行并等待
来源：http://hz.hfpthk.cn/gtoyznrrml.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jianghu66.top/gtkomevkaf.html

[R36] 并发执行多个任务
来源：http://hz.hongshengwenyu.top/gtjxzrvpby.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yangfankeji.com/gtmakiiqbd.html

[R37] 把输出赋给变量
来源：http://hz.cucudq.cn/gtophjipym.html

files=$(ls -1)
来源：http://hz.yvedp.cn/gtowzjzdkr.html

[R38] 管道串联
来源：http://hz.jinqigufen.top/gtzsbidrba.html

cat a.txt | grep -i error | wc -l
来源：http://hz.nanxinkj.top/gtrmdfsucn.html

[R39] 重定向标准输出与错误
来源：http://hz.yj20258888.top/gtdhqtsayk.html

cmd > out.log 2>&1
来源：http://hz.gaohongyu789.top/gtkxfysddt.html

[R40] 追加写日志
来源：http://hz.chenzaomai.com/gtnopsoodj.html

echo "log" >> out.log
来源：http://hz.redwolf501.top/gtwvtrmhht.html

[R41] 丢弃输出
来源：http://hz.sweek.top/gtbfcrsuvn.html

cmd >/dev/null 2>&1
来源：http://hz.fzhhl.top/gtizhpoohm.html

[R42] 输入重定向
来源：http://hz.chenlongwang.top/gtfqbrutlc.html

wc -l < a.txt
来源：http://hz.havefunace.top/gtnqbiwszt.html

[R43] 按名字查找文件
来源：http://hz.smart0.xyz/gtgpcjprlo.html

find . -name "*.log" -type f
来源：http://hz.gogol.net.cn/gtezayfylb.html

[R44] 按修改时间查找
来源：http://hz.jinqigufen.top/gtsuubdrjg.html

find . -mtime -7 -type f
来源：http://hz.hammf.cn/gtfgdkirsn.html

[R45] 批量删除
来源：http://hz.nwbrower.top/gtslzyggmm.html

find . -name "*.tmp" -delete
来源：http://hz.havefunace.top/gtespjsyel.html

[R46] 递归替换文件内容
来源：http://hz.tian-w.cn/gtqyhkagfw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hnqzz.top/gtpwvbcyju.html

[R47] sed 单行替换
来源：http://hz.feifeiyinyue.top/gtydccfxhi.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nanxuanxn.top/gtwzvteewd.html

[R48] awk 取指定列
来源：http://hz.quarkkingdee.top/gtvfqendyv.html

awk '{print $1, $3}' a.txt
来源：http://hz.jiagoushi.top/gtweihdqng.html

[R49] awk 带条件
来源：http://hz.hnqzz.top/gtufbuxggx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jianghu66.top/gtnnprswxl.html

[R50] awk 求和
来源：http://hz.xziqi.cn/gtffrtzmnq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zdqjudy.top/gthhgvymtd.html

[R51] 排序去重取前几
来源：http://hz.jinghuilouyu.cn/gtifjwuyhl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hysaishi.cn/gtinedriif.html

[R52] 统计行数
来源：http://hz.hywenlv.cn/gtwwlvmsys.html

wc -l a.txt
来源：http://hz.birdmap.top/gtxqkfwulv.html

[R53] 查看文件头与实时尾
来源：http://hz.xinyue.icu/gtttonubad.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.kuanghao11.cn/gtdqzfvdvr.html

[R54] 比较两个文件
来源：http://hz.aibaodan.cn/gtsauuylci.html

diff a.txt b.txt
来源：http://hz.hnqzz.top/gtpoalsaqf.html

[R55] 压缩与解压
来源：http://hz.aibaodan.cn/gtigvixuvd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.birdmap.top/gtvvpkroev.html

[R56] 远程拷贝
来源：http://hz.quarkkingdee.top/gtuznvcjaa.html

scp file user@host:/path/
来源：http://hz.hfpthk.cn/gtnppsuyun.html

[R57] 远程执行命令
来源：http://hz.zhixingplan.top/gtupwqsiaf.html

ssh user@host 'uptime'
来源：http://hz.cqqwz.cn/gtqyetmtev.html

[R58] 下载文件
来源：http://hz.jlsjyb.cn/gtqtcqdlmd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cashguo.top/gtamiyvaxc.html

[R59] 发 POST JSON
来源：http://hz.xuanzx.com/gtxvbtujky.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xingfuxueyuan.xyz/gtvtkzkzpm.html

[R60] 只看 HTTP 状态码
来源：http://hz.birdmap.top/gtpgqwivzj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yj202588.top/gtxwxdxejh.html

[R61] 磁盘占用
来源：http://hz.xingfuxueyuan.xyz/gtetzaonhb.html

df -h;  du -sh *
来源：http://hz.hywenlv.cn/gtfmlfkrnn.html

[R62] 找最占空间的文件
来源：http://hz.cdnleiting.top/gthhihqotg.html

du -ah . | sort -rh | head -10
来源：http://hz.yvedp.cn/gtgejmhnja.html

[R63] 内存与进程
来源：http://hz.ppjwa.cn/gtbltjlkqt.html

free -h;  ps aux | grep nginx
来源：http://hz.nwbrower.top/gtgyvebeoj.html

[R64] 结束进程
来源：http://hz.pengpengdd.cyou/gtuyvagsfp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yongpay.top/gtajgxodat.html

[R65] 查看端口占用
来源：http://hz.yuxming.cn/gtwlovpjhb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhongyouzk.top/gtczjonnqh.html

[R66] 定时任务
来源：http://hz.svipenyu.cn/gtuzcpexpa.html

crontab -e;  crontab -l
来源：http://hz.shanyushiyangtech.top/gtsilozfgm.html

[R67] 生成随机十六进制串
来源：http://hz.chenjidiqi.icu/gtpxuvzfki.html

openssl rand -hex 16
来源：http://hz.yangfankeji.com/gttnfyigjp.html

[R68] 计算文件校验值
来源：http://hz.yonumen.top/gtuufiwudb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.smart0.xyz/gtsctyrqcb.html

[R69] 生成随机密码
来源：http://hz.zhaomingkeji.xyz/gtobcbvviu.html


<!-- 参考信息 -->