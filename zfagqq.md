代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.daria6918.cn/gtrzklhibm.html

[Q28] 求和与平均
来源：http://hz.smart0.xyz/gtcuiomifx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ehwqpu.com/gtobzuwpnn.html

[Q29] 最大最小值
来源：http://hz.guowangkeji.top/gtrotcwech.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xylfe.cn/gtmfgvuqli.html

[Q30] 分组统计
来源：http://hz.jyoumei.cn/gtdwtgyjbo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shanyushiyangtech.top/gtecastbhr.html

[Q31] 分组后过滤
来源：http://hz.tanke756.top/gtzfylnliy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hnqzz.top/gtcmlbppnh.html

[Q32] 分组拼接字符串
来源：http://hz.tian-w.cn/gtfszkhfrq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ivvv.top/gtdnbpeqil.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yueranfly.top/gtjqwlddfv.html

[Q33] 多列分组
来源：http://hz.vqdsnc.cn/gtalnggfgh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.0kj1m.cn/gtzocarptu.html

[Q34] 每组取第一条
来源：http://hz.guowangkeji.top/gtfzvikvtd.html

SELECT * FROM (
来源：http://hz.9152youxi.cn/gtgkpazzct.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenjidiqi.icu/gtpdkhkkoi.html

) t WHERE rn = 1;
来源：http://hz.tanke756.top/gtfdqoqrrd.html

[Q35] 内连接
来源：http://hz.nwbrower.top/gtrzsbrixd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.tianlin.xyz/gtabifkbtl.html

[Q36] 左连接
来源：http://hz.gogol.net.cn/gtmejrhozy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.snrcjt.cn/gtilznfkkk.html

[Q37] 右连接
来源：http://hz.cheryme.top/gtrvpfwter.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jianghu66.top/gtamhewgsb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yuxming.cn/gtluuhqkmx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.daxiang520.top/gtpvzooqld.html

[Q39] 自连接（查上下级）
来源：http://hz.kuanghao11.cn/gtfgarftjp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.meibo888.top/gtwysgdhng.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yvedp.cn/gtbocgmtbt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.iojbl.cn/gttnylvuaa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ydzc1.top/gtwwvocrfm.html

[Q41] 多表连接
来源：http://hz.aizwys.cn/gtruypmdox.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jiagoushi.top/gtxlvjplig.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hfpthk.cn/gtdikluewf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.aibaodan.cn/gtfbaexvpq.html

[Q42] 连接条件附加过滤
来源：http://hz.yangfankeji.com/gtdxasgrys.html

SELECT u.name, o.amount FROM users u
来源：http://hz.redwolf501.top/gtksqbcfid.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.feifeiyinyue.top/gtjhnaqelw.html

[Q43] 标量子查询
来源：http://hz.gogol.net.cn/gtsxbumwxw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yonumen.top/gtfvjupkoc.html

[Q44] IN 子查询
来源：http://hz.hammf.cn/gthsmmwnlr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.snrcjt.cn/gtawzzbwqp.html

[Q45] EXISTS 判断存在
来源：http://hz.zhongyouzk.top/gtciadatbj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgufenzy.top/gtvpqxisav.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.redwolf501.top/gthcvmzriw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yanxiufei.cn/gtdymjnmng.html

[Q47] 与平均值比较
来源：http://hz.gaohongyu789.top/gtaeqnbuzh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hongshengwenyu.top/gtztbjdmwi.html

[Q48] CTE 公用表表达式
来源：http://hz.ydjk.org.cn/gtcsfkprpr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shzxlz.cn/gtgfenkjpt.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hywenlv.cn/gtuaamxewd.html

[Q49] 更新单行
来源：http://hz.zhongyouzk.top/gtrtuneatt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenzaomai.com/gtochzapqe.html

[Q50] 批量更新
来源：http://hz.dashuyun.cn/gtgmogtyra.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhongyouzk.top/gtamvtwkaq.html

[Q51] 用子查询更新
来源：http://hz.ppjwa.cn/gtjpgycani.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yvedp.cn/gtsrfwtkog.html

[Q52] 删除指定行
来源：http://hz.jiagoushi.top/gtmbjrnmwj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zycfv.cn/gtqmeutupi.html

[Q53] 按条件删除
来源：http://hz.ivvv.top/gtokawopeh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xuanzx.com/gtkppcnvut.html

[Q54] 清空表
来源：http://hz.wangdashe.top/gtkowkdcdo.html

TRUNCATE TABLE logs;
来源：http://hz.yanxiufei.cn/gtxwoykhou.html

[Q55] 排名（并列占位）
来源：http://hz.redwolf501.top/gtrazvuimk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.wangshuangyany.cn/gtmjsmfxts.html

[Q56] 密集排名（并列不占位）
来源：http://hz.chenjidiqi.icu/gtvdfclbcj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.andypj.xyz/gtrikfuoqp.html

[Q57] 行号
来源：http://hz.chenlongwang.top/gtrikkymxg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shuidangran.top/gtozpbdptu.html

[Q58] 累计求和
来源：http://hz.nanxinkj.top/gttoasrozw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zdqjudy.top/gtsqdojgss.html

[Q59] 分组内累计
来源：http://hz.jyoumei.cn/gtdpispmjl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xziqi.cn/gtwuycysoy.html

[Q60] 取上一行 / 下一行
来源：http://hz.hnqzz.top/gtmdhidlnb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinqigfzy.top/gtmrfjgjkr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.svipenyu.cn/gtfsoxmwxo.html

[Q61] 移动平均
来源：http://hz.zhaomingkeji.xyz/gtvzjwqwnp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yuanzhike.top/gthatwzciw.html

[Q62] 分组占比
来源：http://hz.9152youxi.cn/gtdsgtthhz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jianghu66.top/gtedmcbbnd.html

[Q63] 开启事务
来源：http://hz.nanxinkj.top/gtstnenimy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yueranfly.top/gtiuqryvix.html

[Q64] 提交事务
来源：http://hz.zhiwuduotai.top/gthyycrwua.html

COMMIT;
来源：http://hz.yvedp.cn/gttewejala.html

[Q65] 回滚事务
来源：http://hz.xuetiantiany.cn/gtgqlqtufr.html

ROLLBACK;
来源：http://hz.jinyuanbaomall.cn/gtqjurkobi.html

[Q66] 行锁查询
来源：http://hz.nanxinkj.top/gteowxepxd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yuanzhike.top/gtrlcaiudq.html

[Q67] 设置隔离级别
来源：http://hz.kuanghao11.cn/gtjqkgipsm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.meibo888.top/gtkawtgugz.html

[Q68] 保存点
来源：http://hz.hnxiangtu.top/gtokctbvbh.html

SAVEPOINT sp1;
来源：http://hz.jyoumei.cn/gtvzoxdcus.html

ROLLBACK TO sp1;
来源：http://hz.316326.xyz/gtivxsgsde.html

[Q69] 查看执行计划
来源：http://hz.guowangkeji.top/gtuifqrzka.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gotoacloud.top/gtepjvilgt.html

[Q70] 更新统计信息
来源：http://hz.shuidangran.top/gtqhcnvkoi.html

ANALYZE TABLE users;
来源：http://hz.nanxinkj.top/gtcgvinrzr.html

[Q71] 查看建表语句
来源：http://hz.dashuyun.cn/gthchydxms.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ydjk.org.cn/gttgxozmuc.html

[Q72] 查看索引
来源：http://hz.cdnleiting.top/gtcthjycnx.html

SHOW INDEX FROM users;
来源：http://hz.gaohongyu789.top/gtjnmzqepn.html

[Q73] 查看表状态
来源：http://hz.hnxiangtu.top/gtlyfvkpav.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.0kj1m.cn/gtqyzjvpax.html

[Q74] 强制使用索引
来源：http://hz.c1oappe.top/gtcfeahbox.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ydjk.org.cn/gtoyjktuph.html

[Q75] 日期格式化
来源：http://hz.aibaodan.cn/gtbktgptvf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ydzc1.top/gtwqrzfbdt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hywenlv.cn/gtrnqtfers.html

[Q76] 按天统计
来源：http://hz.zhijiandao.cn/gtdweoaohh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhiwuduotai.top/gthkqbixee.html

[Q77] 时间加减
来源：http://hz.xziqi.cn/gtqaorofzs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhoulong.xyz/gtrxbbmtng.html

[Q78] 当前时间
来源：http://hz.iojbl.cn/gtsosdltvm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xziqi.cn/gtxcypumhk.html

[Q79] 字符串拼接
来源：http://hz.zhixingplan.top/gtejzejqtu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shanyushiyangkeji.top/gtwtjxnhbd.html

[Q80] 字符串截取
来源：http://hz.cdnleiting.top/gtadntxnue.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.316326.xyz/gtyjcvmjtt.html

[Q81] 字符串替换
来源：http://hz.c1oappe.top/gtmhkyfghp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xuetiantiany.cn/gtbxcputma.html

[Q82] 字符长度与字节长度
来源：http://hz.xingfuxueyuan.xyz/gtbauwompm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hnqzz.top/gtopqrdmon.html

[Q83] 大小写转换
来源：http://hz.gogol.net.cn/gtnuxcgsxm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtexztcoat.html

[Q84] 去除首尾空格
来源：http://hz.tian-w.cn/gtetyhofli.html

SELECT TRIM(name) FROM users;
来源：http://hz.hnxiangtu.top/gtrunmttif.html

[Q85] 数值取整
来源：http://hz.yuanzhike.top/gtvcjsuilv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shanyushiyangtech.top/gtcdiaagqb.html

[Q86] 读取 JSON 字段
来源：http://hz.ppjwa.cn/gtcelbregf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hnqzz.top/gtselomnzo.html

[Q87] JSON 字段做条件
来源：http://hz.yongpay.top/gtlodhashb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guowangkeji.top/gtxugxnrxh.html

[Q88] 行转列（条件聚合）
来源：http://hz.pengpengdd.cyou/gtgsdfzujc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.smart0.xyz/gtjydnpvnm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yj202588.top/gtmjzxgvbw.html

[Q89] 判断表是否存在
来源：http://hz.316326.xyz/gtkrununzw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yongpay.top/gtbrvlnxzi.html

[Q90] 生成序号列
来源：http://hz.ehwqpu.com/gtmhmyjfyd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.mhx1999.top/gtvzekzgcx.html

================================================================================
来源：http://hz.yvedp.cn/gtzfbuhugn.html

R. Bash 专题
来源：http://hz.daxiang520.top/gtfcufkyxb.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtsulwasuu.html

[R01] shebang 与严格模式
来源：http://hz.jqgfzy.top/gtjsoksflk.html

#!/usr/bin/env bash
来源：http://hz.tian-w.cn/gttywbcscr.html

set -euo pipefail
来源：http://hz.nwbrower.top/gtidhjjawe.html

[R02] 变量赋值与使用
来源：http://hz.kuanghao11.cn/gtrbxlqbks.html

name="Tom"; echo "$name"
来源：http://hz.gaohongyu789.top/gtrtjlftuy.html

[R03] 只读变量
来源：http://hz.vqdsnc.cn/gthhvaifjz.html

readonly PI=3.14
来源：http://hz.zhijiandao.cn/gtukkcxowj.html

[R04] 位置参数
来源：http://hz.yanxiufei.cn/gtuwsgrayu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cqqwz.cn/gttffbyzbq.html

[R05] 参数默认值
来源：http://hz.vqdsnc.cn/gthnpgendv.html

name="${1:-default}"
来源：http://hz.pycfn.com/gtllugsuec.html

[R06] 判断命令是否存在
来源：http://hz.daria6918.cn/gtqhyiocfk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.redwolf501.top/gtoqyvpuhm.html

[R07] if 判断文件
来源：http://hz.chenjidiqi.icu/gtobvrslof.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ydzc1.top/gtnlgtnnxq.html

[R08] 数值比较
来源：http://hz.316326.xyz/gtwgnrbfti.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jianghu66.top/gtucybhsep.html

[R09] 字符串比较
来源：http://hz.xuanzx.com/gtjydhtxfh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yonumen.top/gtrkbdnulh.html

[R10] 正则匹配
来源：http://hz.0kj1m.cn/gtkdowzivz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hongshengwenyu.top/gtjguczhxe.html

[R11] case 多分支
来源：http://hz.aizwys.cn/gtrokxbytz.html

case "$1" in
来源：http://hz.jinyuanbaomall.cn/gtsgpiwzep.html

start) echo "启动" ;;
来源：http://hz.nanxuanxn.top/gttychcxmz.html

stop)  echo "停止" ;;
来源：http://hz.snrcjt.cn/gtqbmhzbku.html

*)     echo "未知命令" ;;
来源：http://hz.ehwqpu.com/gthcpbuxoj.html

esac
来源：http://hz.ybcxt.top/gtpzyflxkg.html

[R12] for 遍历文件
来源：http://hz.gotoacloud.top/gtfwodxgld.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hywenlv.cn/gtjpaolidm.html

[R13] for 计数循环
来源：http://hz.nwbrower.top/gtmvakrbwe.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yvedp.cn/gtqvtkpvao.html

[R14] C 风格 for
来源：http://hz.gogol.net.cn/gtrfueqnos.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ydzc1.top/gtmolsgqsr.html

[R15] while 逐行读文件
来源：http://hz.pycfn.com/gtesmmgclm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xylfe.cn/gtqypitjym.html

[R16] until 等待条件
来源：http://hz.pycfn.com/gtoatqfrkz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gotoacloud.top/gtegpjwpoj.html

[R17] 数组定义与取值
来源：http://hz.yuanzhike.top/gtpgxtfzaq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yvedp.cn/gtombwhmmg.html

[R18] 遍历数组
来源：http://hz.hywenlv.cn/gtewglfxcs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.feifeiyinyue.top/gtqxjzznzl.html

[R19] 数组长度
来源：http://hz.jyoumei.cn/gtygputebm.html

echo "${#arr[@]}"
来源：http://hz.haohaochexian.top/gtmlkdkmvd.html

[R20] 关联数组（字典）
来源：http://hz.vqdsnc.cn/gtjxhqpbvo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.daxiang520.top/gtotrldasz.html

[R21] 字符串长度
来源：http://hz.hywenlv.cn/gtltestvzw.html

echo "${#s}"
来源：http://hz.shuidangran.top/gtnysfsdgq.html

[R22] 截取子串
来源：http://hz.chenjidiqi.icu/gtvoltvjgh.html

echo "${s:0:5}"
来源：http://hz.shzxlz.cn/gtfrtacvhw.html

[R23] 字符串替换
来源：http://hz.birdmap.top/gtlbnuxdmw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.svipenyu.cn/gttyfupruj.html

[R24] 大小写转换
来源：http://hz.mhx1999.top/gtpkjmsyfk.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yvedp.cn/gtijyddphc.html

[R25] 去后缀 / 去前缀
来源：http://hz.ppjwa.cn/gtneugjfro.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.tian-w.cn/gtkaanvzqg.html

[R26] 命令替换
来源：http://hz.yuanzhike.top/gtztkwcnms.html

now=$(date +%F); echo "$now"
来源：http://hz.yangfankeji.com/gthimnuyzs.html

[R27] 算术展开
来源：http://hz.mhx1999.top/gtrehsaibp.html

echo $((1 + 2 * 3))
来源：http://hz.yangfankeji.com/gtfwnexdgb.html

[R28] 浮点运算
来源：http://hz.shanyushiyangkeji.top/gtkbivanub.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhijiandao.cn/gtxitzxljm.html

[R29] 定义函数
来源：http://hz.shangyingyoupin.top/gtkjrqlezk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.dianchejie.cn/gtiufozlsx.html

[R30] 函数返回状态码
来源：http://hz.nanxinkj.top/gtzpfaqmdc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ybcxt.top/gtjxgbmyiy.html

[R31] 局部变量
来源：http://hz.zhijiandao.cn/gtlrloozko.html

f() { local x=1; echo "$x"; }
来源：http://hz.tanke756.top/gtwtlgcnuw.html

[R32] 参数个数校验
来源：http://hz.cdnleiting.top/gtiseaacki.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.kuanghao11.cn/gtnxxmutwo.html

[R33] 捕获错误并提示行号
来源：http://hz.guannengcc.top/gtyueyvlsd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xuetiantiany.cn/gtjhcieper.html

[R34] 退出时清理
来源：http://hz.yj202588.top/gtgzndaubq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gtkxuladvu.html

[R35] 后台执行并等待
来源：http://hz.aibaodan.cn/gtywtlrddv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xuetiantiany.cn/gtzqosljep.html

[R36] 并发执行多个任务
来源：http://hz.feifeiyinyue.top/gtpguzomib.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ydjk.org.cn/gtjqtewpjp.html

[R37] 把输出赋给变量
来源：http://hz.fzhhl.top/gtfyafodpn.html

files=$(ls -1)
来源：http://hz.cqqwz.cn/gtujtiwthd.html

[R38] 管道串联
来源：http://hz.dianchejie.cn/gtinpaesoa.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhengqikj.top/gtxmrzfwdg.html

[R39] 重定向标准输出与错误
来源：http://hz.feifeiyinyue.top/gtqebhxqjx.html

cmd > out.log 2>&1
来源：http://hz.guannengcc.top/gtofthjhex.html

[R40] 追加写日志
来源：http://hz.iojbl.cn/gtgupnyadk.html

echo "log" >> out.log
来源：http://hz.pycfn.com/gtkrmtqwab.html

[R41] 丢弃输出
来源：http://hz.gaohongyu789.top/gtrbhgluiu.html

cmd >/dev/null 2>&1
来源：http://hz.xinyue.icu/gtbigoaalf.html

[R42] 输入重定向
来源：http://hz.gzhubu.top/gtuiogwphm.html

wc -l < a.txt
来源：http://hz.xingfuxueyuan.xyz/gtqcigfvxt.html

[R43] 按名字查找文件
来源：http://hz.xuanzx.com/gtwgqprvfd.html

find . -name "*.log" -type f
来源：http://hz.xziqi.cn/gtekvhnnxy.html

[R44] 按修改时间查找
来源：http://hz.yueranfly.top/gtvnlmcnwb.html

find . -mtime -7 -type f
来源：http://hz.jqgfzy.top/gtspygfopf.html

[R45] 批量删除
来源：http://hz.wangdashe.top/gtlcvhbdxu.html

find . -name "*.tmp" -delete
来源：http://hz.vqdsnc.cn/gtkmtmmbgk.html

[R46] 递归替换文件内容
来源：http://hz.nanxinkj.top/gtqiglncxj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ywan-chungtsiang.top/gtrdvnrglw.html

[R47] sed 单行替换
来源：http://hz.havefunace.top/gtcquxpkxp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xziqi.cn/gtboidltjn.html

[R48] awk 取指定列
来源：http://hz.snrcjt.cn/gtisaayuid.html

awk '{print $1, $3}' a.txt
来源：http://hz.guannengcc.top/gtnmrfisle.html

[R49] awk 带条件
来源：http://hz.sxryk.cn/gtbjcjawje.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shzxlz.cn/gtbbnuyqjh.html

[R50] awk 求和
来源：http://hz.havefunace.top/gtgylfwyjb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sxryk.cn/gtwbexuapi.html

[R51] 排序去重取前几
来源：http://hz.dianchejie.cn/gtyxjewzgn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.aizwys.cn/gtdqhdttni.html

[R52] 统计行数
来源：http://hz.birdmap.top/gtfcsofmub.html

wc -l a.txt
来源：http://hz.yanxiufei.cn/gtwolrkpcr.html

[R53] 查看文件头与实时尾
来源：http://hz.zhaomingkeji.xyz/gtmtniymqs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ivvv.top/gtqxiexzvh.html

[R54] 比较两个文件
来源：http://hz.jianghu66.top/gtkldqmgzh.html

diff a.txt b.txt
来源：http://hz.hnqzz.top/gtilspqtuf.html

[R55] 压缩与解压
来源：http://hz.gzhubu.top/gtyvxugalr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xingfuxueyuan.xyz/gtiludeusn.html

[R56] 远程拷贝
来源：http://hz.ivvv.top/gtnxrobnpc.html

scp file user@host:/path/
来源：http://hz.bjfxy.top/gtjwcgxvkx.html

[R57] 远程执行命令
来源：http://hz.jqgufenzy.top/gtdtimjzxk.html

ssh user@host 'uptime'
来源：http://hz.nwbrower.top/gtomdangax.html

[R58] 下载文件
来源：http://hz.smart0.xyz/gtpbrfvpro.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yuanzhike.top/gttjpeefoy.html

[R59] 发 POST JSON
来源：http://hz.ehwqpu.com/gthcnwamum.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hfpthk.cn/gtlyltbhdm.html

[R60] 只看 HTTP 状态码
来源：http://hz.c1oappe.top/gtuynlrabr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nwbrower.top/gtstpkcdxl.html

[R61] 磁盘占用
来源：http://hz.kuanghao11.cn/gtmtjjigbi.html

df -h;  du -sh *
来源：http://hz.tanke756.top/gtazkyioqk.html

[R62] 找最占空间的文件
来源：http://hz.shuidangran.top/gtyrawiwkt.html

du -ah . | sort -rh | head -10
来源：http://hz.cashguo.top/gtwzpvuixe.html

[R63] 内存与进程
来源：http://hz.fengsongda.top/gtgpgrblkl.html

free -h;  ps aux | grep nginx
来源：http://hz.dianchejie.cn/gtkoougkwr.html

[R64] 结束进程
来源：http://hz.feifeiyinyue.top/gtavkbxiiw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xingfuxueyuan.xyz/gtienwcqln.html

[R65] 查看端口占用
来源：http://hz.shanyushiyangkeji.top/gtmhudgvek.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.meibo888.top/gtwxymnowz.html

[R66] 定时任务
来源：http://hz.iojbl.cn/gtnhofhryg.html

crontab -e;  crontab -l
来源：http://hz.fzhhl.top/gtdgnciqry.html

[R67] 生成随机十六进制串
来源：http://hz.sxryk.cn/gtzfjpowvq.html

openssl rand -hex 16
来源：http://hz.pengpengdd.cyou/gthnrelaii.html

[R68] 计算文件校验值
来源：http://hz.sysykeji.top/gtjnviozhl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.smart0.xyz/gtmwijkcej.html

[R69] 生成随机密码
来源：http://hz.hammf.cn/gtilflqeim.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhixingplan.top/gttsgyfbdb.html

[R70] 时间戳与互转
来源：http://hz.cashguo.top/gtxuqsvexb.html

date +%s;  date -d @1700000000
来源：http://hz.feifeiyinyue.top/gtclhljtxh.html

[R71] 日期格式化
来源：http://hz.jyoumei.cn/gtjnlybqdj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gzhubu.top/gtigduyald.html

[R72] 等待端口就绪
来源：http://hz.dianchejie.cn/gtttftymkf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zdqjudy.top/gtmzeyqzdn.html

[R73] 分割大日志
来源：http://hz.havefunace.top/gtaiaqazjs.html

split -l 1000 big.log part_
来源：http://hz.xuetiantiany.cn/gtmcvfmbae.html

[R74] 批量重命名
来源：http://hz.guowangkeji.top/gtjaqteaca.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.meibo888.top/gtehkougyn.html

[R75] 导出环境变量
来源：http://hz.sysykeji.top/gtczyudedl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jqgufenzy.top/gtxuslxjww.html

[R76] 使用临时文件
来源：http://hz.chenjidiqi.icu/gtxacjscto.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cashguo.top/gtsfvafvpb.html

[R77] 读取用户输入
来源：http://hz.jianghu66.top/gtkjxbnllg.html


<!-- 参考信息 -->