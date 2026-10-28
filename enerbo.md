代发 wailian999

SELECT * FROM users;
来源：http://hz.ywan-chungtsiang.top/gtpfuhuqns.html

[Q16] 查询指定列
来源：http://hz.316326.xyz/gtzneoqhfe.html

SELECT id, name FROM users;
来源：http://hz.zdqjudy.top/gtowfivxxu.html

[Q17] 条件查询
来源：http://hz.yueranfly.top/gtpkertqku.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhongyouzk.top/gtbiijtnaz.html

[Q18] 模糊匹配
来源：http://hz.yueranfly.top/gtcametfca.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.bjfxy.top/gtxdibrujc.html

[Q19] 范围查询
来源：http://hz.gotoacloud.top/gtcwaaukwb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.guannengcc.top/gtlglrkejf.html

[Q20] IN 列表
来源：http://hz.shuidangran.top/gtrayaibpo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hnxiangtu.top/gtgbykljbs.html

[Q21] 空值判断
来源：http://hz.yangfankeji.com/gttdazelar.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.nwbrower.top/gtwzixraux.html

[Q22] 排序
来源：http://hz.yanxiufei.cn/gtxofnmnhd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinghuilouyu.cn/gtrhdqosju.html

[Q23] 分页
来源：http://hz.gotoacloud.top/gthvxhofyn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sufxvd.cn/gtvhrpdbpj.html

[Q24] 去重
来源：http://hz.ehwqpu.com/gtrivfryqo.html

SELECT DISTINCT city FROM users;
来源：http://hz.chenzaomai.com/gtlxvhcuzm.html

[Q25] 只取前 N 条
来源：http://hz.svipenyu.cn/gthvrrhhwk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhiwuduotai.top/gtaqjkwjci.html

[Q26] 计数
来源：http://hz.cucudq.cn/gtbdbsajtm.html

SELECT COUNT(*) FROM users;
来源：http://hz.daxiang520.top/gtmghjmbfb.html

[Q27] 条件计数
来源：http://hz.sweek.top/gtwkkxqbqt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pengpengdd.cyou/gtdoxkvyjz.html

[Q28] 求和与平均
来源：http://hz.hywenlv.cn/gtrvblvnoz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xuetiantiany.cn/gtujtvtuec.html

[Q29] 最大最小值
来源：http://hz.redwolf501.top/gtwgmmhyhi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtrekhlzst.html

[Q30] 分组统计
来源：http://hz.cucudq.cn/gtcueurlvc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gtdwqtksez.html

[Q31] 分组后过滤
来源：http://hz.aibaodan.cn/gteaojvdxw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shanyushiyangkeji.top/gtynoamafy.html

[Q32] 分组拼接字符串
来源：http://hz.zhengqikj.top/gtgntsizme.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hongshengwenyu.top/gtnjxowrnp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.tian-w.cn/gtidtxpwad.html

[Q33] 多列分组
来源：http://hz.cdnleiting.top/gttgtggdlx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daria6918.cn/gtkjjyksrb.html

[Q34] 每组取第一条
来源：http://hz.zycfv.cn/gtmgleuuvm.html

SELECT * FROM (
来源：http://hz.zdqjudy.top/gtdymrvbic.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xziqi.cn/gtnfyrunll.html

) t WHERE rn = 1;
来源：http://hz.ydjk.org.cn/gtvuwphdig.html

[Q35] 内连接
来源：http://hz.jyoumei.cn/gtmaqbfyga.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zycfv.cn/gtshnhndlr.html

[Q36] 左连接
来源：http://hz.cdnleiting.top/gtnsrjbmbv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuetiantiany.cn/gtystblgjp.html

[Q37] 右连接
来源：http://hz.xuanzx.com/gtblnoknqb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenzaomai.com/gtxgqszdya.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sweek.top/gtwcuolgwu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.iojbl.cn/gtmszghlhd.html

[Q39] 自连接（查上下级）
来源：http://hz.ppjwa.cn/gtlqymdiwq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.chenjidiqi.icu/gtnemnlvqp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.smart0.xyz/gtbcogjjxa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.aibaodan.cn/gteeptojrb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinqigfzy.top/gtykolfinr.html

[Q41] 多表连接
来源：http://hz.sufxvd.cn/gtwfqyhgou.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ydjk.org.cn/gtsjqcqpzu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhaomingkeji.xyz/gtrylimebb.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hammf.cn/gtoiwkaiba.html

[Q42] 连接条件附加过滤
来源：http://hz.quarkkingdee.top/gthvbiipss.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cqqwz.cn/gtddzbfhvg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zycfv.cn/gtadiqcvrf.html

[Q43] 标量子查询
来源：http://hz.ehwqpu.com/gtvrrkkjxb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gzhubu.top/gtbpkqtgrr.html

[Q44] IN 子查询
来源：http://hz.jiagoushi.top/gtfuwqorvd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinqigfzy.top/gtwiezblzy.html

[Q45] EXISTS 判断存在
来源：http://hz.xylfe.cn/gthedawnek.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.kuanghao11.cn/gtozskihxh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj20258.top/gtfbglpyef.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hongshengwenyu.top/gteqinizcy.html

[Q47] 与平均值比较
来源：http://hz.yuxming.cn/gtyjeexggn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jyoumei.cn/gtpbcedyav.html

[Q48] CTE 公用表表达式
来源：http://hz.hysaishi.cn/gthazvkung.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinqigfzy.top/gtfenfasqq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.fzhhl.top/gtsyxswsyv.html

[Q49] 更新单行
来源：http://hz.bjfxy.top/gtzphrdaai.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.0kj1m.cn/gtrfmtwuko.html

[Q50] 批量更新
来源：http://hz.jinghuilouyu.cn/gtygfazmbf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gogol.net.cn/gtdkledmhq.html

[Q51] 用子查询更新
来源：http://hz.yueranfly.top/gtkklzbxbp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.daria6918.cn/gtdcyjdlro.html

[Q52] 删除指定行
来源：http://hz.nanxinkj.top/gtfwfgtvyc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gotoacloud.top/gtushqapbt.html

[Q53] 按条件删除
来源：http://hz.jqgufenzy.top/gtvunqjcvx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.316326.xyz/gtnbywpycn.html

[Q54] 清空表
来源：http://hz.yueranfly.top/gtfihkzceo.html

TRUNCATE TABLE logs;
来源：http://hz.tian-w.cn/gtkqqfmuyz.html

[Q55] 排名（并列占位）
来源：http://hz.jiagoushi.top/gtesvpmyhe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yuanzhike.top/gtxxlfropz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.9152youxi.cn/gtkfckehqc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xuanzx.com/gtkjqthtlo.html

[Q57] 行号
来源：http://hz.gaohongyu789.top/gtdabiyfuf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.mhx1999.top/gtuarxeslu.html

[Q58] 累计求和
来源：http://hz.52xcode.cn/gtlfdpxmzr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.kuanghao11.cn/gtozfwgxmf.html

[Q59] 分组内累计
来源：http://hz.aibaodan.cn/gtgngjjtcl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nanxinkj.top/gtllvglgti.html

[Q60] 取上一行 / 下一行
来源：http://hz.cashguo.top/gtypcpjxxd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.dashuyun.cn/gtjxgkjpem.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.mhx1999.top/gtonjxytjw.html

[Q61] 移动平均
来源：http://hz.yj202588.top/gtyzylvwll.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zycfv.cn/gtshdxwiks.html

[Q62] 分组占比
来源：http://hz.yongpay.top/gtnjereggc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtpiivgnjw.html

[Q63] 开启事务
来源：http://hz.yj20258888.top/gtaqjihzbu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yj20258.top/gttvdjxkek.html

[Q64] 提交事务
来源：http://hz.snrcjt.cn/gthwrvzmvz.html

COMMIT;
来源：http://hz.zycfv.cn/gtoemjwooi.html

[Q65] 回滚事务
来源：http://hz.fzhhl.top/gtiopcxgit.html

ROLLBACK;
来源：http://hz.cqqwz.cn/gtilydvlmu.html

[Q66] 行锁查询
来源：http://hz.shanyushiyangkeji.top/gtvjmsqyfk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.andypj.xyz/gtwpvmirwb.html

[Q67] 设置隔离级别
来源：http://hz.c1oappe.top/gtorehcisv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhiwuduotai.top/gtdxxhfslp.html

[Q68] 保存点
来源：http://hz.gzhubu.top/gtpxsfnhov.html

SAVEPOINT sp1;
来源：http://hz.hnqzz.top/gtvdjovwba.html

ROLLBACK TO sp1;
来源：http://hz.birdmap.top/gtsjyfibey.html

[Q69] 查看执行计划
来源：http://hz.fengsongda.top/gtlhrqbsvo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shanyushiyangtech.top/gtzusayqmt.html

[Q70] 更新统计信息
来源：http://hz.ydjk.org.cn/gtzqntwgwb.html

ANALYZE TABLE users;
来源：http://hz.yuanzhike.top/gtnmhfjvec.html

[Q71] 查看建表语句
来源：http://hz.tianlin.xyz/gtpbpprogv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.wangdashe.top/gtaegvyqez.html

[Q72] 查看索引
来源：http://hz.shuidangran.top/gthrhvhfwj.html

SHOW INDEX FROM users;
来源：http://hz.jinqigfzy.top/gtneyfsovt.html

[Q73] 查看表状态
来源：http://hz.feifeiyinyue.top/gtwypjhzyr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sysykeji.top/gtglvsfjlg.html

[Q74] 强制使用索引
来源：http://hz.sufxvd.cn/gtuycoguvw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sysykeji.top/gtarkjwhom.html

[Q75] 日期格式化
来源：http://hz.hnqzz.top/gtfhbsycur.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cqqwz.cn/gtjamgsijh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.bjfxy.top/gtiytilwip.html

[Q76] 按天统计
来源：http://hz.ybcxt.top/gtnmlcxlbk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jlsjyb.cn/gtdftuduzy.html

[Q77] 时间加减
来源：http://hz.jqgufenzy.top/gtixzzveyx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.c1oappe.top/gtcjjsxsge.html

[Q78] 当前时间
来源：http://hz.yanxiufei.cn/gtuboowoji.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cdnleiting.top/gtclksufwu.html

[Q79] 字符串拼接
来源：http://hz.quarkkingdee.top/gtpupecqtd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.kuanghao11.cn/gtycksials.html

[Q80] 字符串截取
来源：http://hz.zhoulong.xyz/gtrektjwmm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.redwolf501.top/gtgygnpszg.html

[Q81] 字符串替换
来源：http://hz.sxryk.cn/gtsewvrpqb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xinyue.icu/gtweudhiml.html

[Q82] 字符长度与字节长度
来源：http://hz.chenzaomai.com/gtnvhvlaoi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yueranfly.top/gtganlabqt.html

[Q83] 大小写转换
来源：http://hz.jinqigufen.top/gtgubopbmv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.iojbl.cn/gtsedogkgl.html

[Q84] 去除首尾空格
来源：http://hz.0kj1m.cn/gtyeclkwer.html

SELECT TRIM(name) FROM users;
来源：http://hz.sweek.top/gtfyeacigv.html

[Q85] 数值取整
来源：http://hz.ivvv.top/gtcikabirc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.sufxvd.cn/gtkonoqnvi.html

[Q86] 读取 JSON 字段
来源：http://hz.hnqzz.top/gtmqavqucf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.bjfxy.top/gtkhplxztg.html

[Q87] JSON 字段做条件
来源：http://hz.ybcxt.top/gtatdfywky.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.mhx1999.top/gtnnuzozww.html

[Q88] 行转列（条件聚合）
来源：http://hz.xuetiantiany.cn/gtexrgxdol.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.guannengcc.top/gtogovykgo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ppjwa.cn/gtmctiyzsl.html

[Q89] 判断表是否存在
来源：http://hz.wangdashe.top/gtfdrastve.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.birdmap.top/gthxzncmzs.html

[Q90] 生成序号列
来源：http://hz.hnqzz.top/gtitdiwkgv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.wangdashe.top/gtezzizuyi.html

================================================================================
来源：http://hz.guowangkeji.top/gtvhpujqyx.html

R. Bash 专题
来源：http://hz.zycfv.cn/gthcaozulm.html

================================================================================
来源：http://hz.c1oappe.top/gtvpzeupse.html

[R01] shebang 与严格模式
来源：http://hz.cdnleiting.top/gtuphedlfd.html

#!/usr/bin/env bash
来源：http://hz.cheryme.top/gtmlmtanhg.html

set -euo pipefail
来源：http://hz.kuanghao11.cn/gtgxpagyxs.html

[R02] 变量赋值与使用
来源：http://hz.jqgufenzy.top/gtgnpsaczm.html

name="Tom"; echo "$name"
来源：http://hz.cdnleiting.top/gtztxxielw.html

[R03] 只读变量
来源：http://hz.tanke756.top/gthwsjjpnu.html

readonly PI=3.14
来源：http://hz.yj20258888.top/gtekcmvmno.html

[R04] 位置参数
来源：http://hz.xinyue.icu/gtxxxwthve.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hammf.cn/gtmffprpqx.html

[R05] 参数默认值
来源：http://hz.hammf.cn/gtzzscqlde.html

name="${1:-default}"
来源：http://hz.yuxming.cn/gthmdjtfqn.html

[R06] 判断命令是否存在
来源：http://hz.xuetiantiany.cn/gtjquswjac.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ywan-chungtsiang.top/gtlsqmxjgk.html

[R07] if 判断文件
来源：http://hz.cucudq.cn/gtiiivzhyj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sweek.top/gtivwjglsm.html

[R08] 数值比较
来源：http://hz.redwolf501.top/gtthpxzaug.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinqigufen.top/gtztrvwxth.html

[R09] 字符串比较
来源：http://hz.jinqigufen.top/gtjyryapri.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.fengsongda.top/gtzfmekbsl.html

[R10] 正则匹配
来源：http://hz.birdmap.top/gtncudnrkx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinghuilouyu.cn/gtnglhefom.html

[R11] case 多分支
来源：http://hz.zycfv.cn/gtnieelcal.html

case "$1" in
来源：http://hz.xuanzx.com/gtghdwpycl.html

start) echo "启动" ;;
来源：http://hz.daxiang520.top/gtrzggvwqt.html

stop)  echo "停止" ;;
来源：http://hz.jianghu66.top/gtdrxtblzg.html

*)     echo "未知命令" ;;
来源：http://hz.iojbl.cn/gtuwrkxadh.html

esac
来源：http://hz.quarkkingdee.top/gtglnskgrf.html

[R12] for 遍历文件
来源：http://hz.316326.xyz/gtqphizlst.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ybcxt.top/gtxklwfzkv.html

[R13] for 计数循环
来源：http://hz.redwolf501.top/gtxkioijiu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj20258.top/gtwigdsasq.html

[R14] C 风格 for
来源：http://hz.shanyushiyangtech.top/gtusaikakp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zycfv.cn/gtumcbrfgw.html

[R15] while 逐行读文件
来源：http://hz.yuanzhike.top/gtvdeiveuz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gaohongyu789.top/gtdewvtjuf.html

[R16] until 等待条件
来源：http://hz.sufxvd.cn/gtuyrypgjs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yuxming.cn/gtrbalfnwm.html

[R17] 数组定义与取值
来源：http://hz.nwbrower.top/gtxtoxjhle.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sufxvd.cn/gtezubwizp.html

[R18] 遍历数组
来源：http://hz.pycfn.com/gtiapdjpkz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.smart0.xyz/gtavhkvptw.html

[R19] 数组长度
来源：http://hz.shzxlz.cn/gtktfucfcb.html

echo "${#arr[@]}"
来源：http://hz.zycfv.cn/gtptjsszlo.html

[R20] 关联数组（字典）
来源：http://hz.yj20258.top/gtlhczsebn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.vqdsnc.cn/gtksggzgzz.html

[R21] 字符串长度
来源：http://hz.yonumen.top/gtxsaxliuk.html

echo "${#s}"
来源：http://hz.xinyue.icu/gtpsxlucld.html

[R22] 截取子串
来源：http://hz.snrcjt.cn/gtxxaqumnf.html

echo "${s:0:5}"
来源：http://hz.jinqigufen.top/gtmwgxarfs.html

[R23] 字符串替换
来源：http://hz.snrcjt.cn/gtifhkvnij.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhoulong.xyz/gtwiwqbkhk.html

[R24] 大小写转换
来源：http://hz.wangdashe.top/gtgvegcska.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenjidiqi.icu/gtqtohfdbx.html

[R25] 去后缀 / 去前缀
来源：http://hz.bjfxy.top/gtatapqxle.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhixingplan.top/gtesqlyyfk.html

[R26] 命令替换
来源：http://hz.sxryk.cn/gtqaukomcm.html

now=$(date +%F); echo "$now"
来源：http://hz.xingfuxueyuan.xyz/gtyslclkxg.html

[R27] 算术展开
来源：http://hz.tian-w.cn/gthrgobdta.html

echo $((1 + 2 * 3))
来源：http://hz.chenlongwang.top/gtptuwhegt.html

[R28] 浮点运算
来源：http://hz.guowangkeji.top/gtflohgyav.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhengqikj.top/gtwxxkjwox.html

[R29] 定义函数
来源：http://hz.kuanghao11.cn/gtbfgwsuad.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.fengsongda.top/gtvdwyxiib.html

[R30] 函数返回状态码
来源：http://hz.chenlongwang.top/gtmtyenmaj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.haohaochexian.top/gtmvoztkga.html

[R31] 局部变量
来源：http://hz.fzhhl.top/gtmqbociri.html

f() { local x=1; echo "$x"; }
来源：http://hz.meibo888.top/gtfuyfasad.html

[R32] 参数个数校验
来源：http://hz.havefunace.top/gthoyjcotd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gogol.net.cn/gtesmiwimg.html

[R33] 捕获错误并提示行号
来源：http://hz.sxryk.cn/gtocpqfunb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.birdmap.top/gtshchkwnv.html

[R34] 退出时清理
来源：http://hz.zhoulong.xyz/gtkklgydfu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.feifeiyinyue.top/gtgdvvuulc.html

[R35] 后台执行并等待
来源：http://hz.pengpengdd.cyou/gtfwoyhhqc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tanke756.top/gtsdljpsco.html

[R36] 并发执行多个任务
来源：http://hz.fzhhl.top/gtxqmuvqtn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.haohaochexian.top/gtgprrdqet.html

[R37] 把输出赋给变量
来源：http://hz.dianchejie.cn/gtioropxeu.html

files=$(ls -1)
来源：http://hz.jianghu66.top/gtaorbikul.html

[R38] 管道串联
来源：http://hz.shanyushiyangkeji.top/gtmollzbsl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.kuanghao11.cn/gtasgfikwu.html

[R39] 重定向标准输出与错误
来源：http://hz.nanxinkj.top/gtqndnnnqj.html

cmd > out.log 2>&1
来源：http://hz.pengpengdd.cyou/gtppaknnpp.html

[R40] 追加写日志
来源：http://hz.hongshengwenyu.top/gtrfmdsico.html

echo "log" >> out.log
来源：http://hz.gzhubu.top/gtvlievcqr.html

[R41] 丢弃输出
来源：http://hz.hongshengwenyu.top/gthwhemndt.html

cmd >/dev/null 2>&1
来源：http://hz.gogol.net.cn/gtwezcslhb.html

[R42] 输入重定向
来源：http://hz.zycfv.cn/gtpdbndovt.html

wc -l < a.txt
来源：http://hz.daria6918.cn/gtbyreihcq.html

[R43] 按名字查找文件
来源：http://hz.zycfv.cn/gtvqldyyik.html

find . -name "*.log" -type f
来源：http://hz.zhaomingkeji.xyz/gtfrffpjdn.html

[R44] 按修改时间查找
来源：http://hz.daria6918.cn/gtylfepqhm.html

find . -mtime -7 -type f
来源：http://hz.aibaodan.cn/gtmmixegzo.html

[R45] 批量删除
来源：http://hz.iojbl.cn/gtfhkjajdf.html

find . -name "*.tmp" -delete
来源：http://hz.shzxlz.cn/gtedbjyxvp.html

[R46] 递归替换文件内容
来源：http://hz.xinyue.icu/gtusmfdzfz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinqigfzy.top/gtyncyihle.html

[R47] sed 单行替换
来源：http://hz.iojbl.cn/gtftynlcvo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sufxvd.cn/gthotejyxm.html

[R48] awk 取指定列
来源：http://hz.snrcjt.cn/gtwoqdkjlp.html

awk '{print $1, $3}' a.txt
来源：http://hz.bjfxy.top/gtgnjsiuoi.html

[R49] awk 带条件
来源：http://hz.wangshuangyany.cn/gtipinuamd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.iojbl.cn/gtrtwbuicp.html

[R50] awk 求和
来源：http://hz.guowangkeji.top/gtusprwmvd.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinghuilouyu.cn/gtjwdwfivr.html

[R51] 排序去重取前几
来源：http://hz.snrcjt.cn/gtditrphph.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.nwbrower.top/gtvcfabotv.html

[R52] 统计行数
来源：http://hz.ywan-chungtsiang.top/gtelecklum.html

wc -l a.txt
来源：http://hz.cheryme.top/gtjuhnfpcz.html

[R53] 查看文件头与实时尾
来源：http://hz.xuanzx.com/gtvkhiqjum.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shangyingyoupin.top/gtgncxwjqe.html

[R54] 比较两个文件
来源：http://hz.sysykeji.top/gtrpwbfvzw.html

diff a.txt b.txt
来源：http://hz.cucudq.cn/gtqkdkrymi.html

[R55] 压缩与解压
来源：http://hz.quarkkingdee.top/gtmrzdrnln.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.daria6918.cn/gtvgiakmfe.html

[R56] 远程拷贝
来源：http://hz.xuanzx.com/gtnbczeijb.html

scp file user@host:/path/
来源：http://hz.feifeiyinyue.top/gtzzqkqmkt.html

[R57] 远程执行命令
来源：http://hz.ppjwa.cn/gtfydmhuee.html

ssh user@host 'uptime'
来源：http://hz.fengsongda.top/gtunhflcyg.html

[R58] 下载文件
来源：http://hz.yj20258888.top/gtcqrjdidu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.guowangkeji.top/gttlfruuai.html

[R59] 发 POST JSON
来源：http://hz.dianchejie.cn/gtptifqjan.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.chenjidiqi.icu/gtukocjtuo.html

[R60] 只看 HTTP 状态码
来源：http://hz.jqgfzy.top/gtyoymwcxy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hongshengwenyu.top/gtmmzphrdo.html

[R61] 磁盘占用
来源：http://hz.meibo888.top/gttnwlmzvi.html

df -h;  du -sh *
来源：http://hz.nanxinkj.top/gtdbledodo.html

[R62] 找最占空间的文件
来源：http://hz.gzhubu.top/gtbrtrvzux.html

du -ah . | sort -rh | head -10
来源：http://hz.xingfuxueyuan.xyz/gtorjylfic.html

[R63] 内存与进程
来源：http://hz.cqqwz.cn/gtzrdpvpwe.html

free -h;  ps aux | grep nginx
来源：http://hz.jlsjyb.cn/gtbpurhuds.html

[R64] 结束进程
来源：http://hz.xingfuxueyuan.xyz/gtniwgqcfm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hywenlv.cn/gtshlavkds.html

[R65] 查看端口占用
来源：http://hz.xziqi.cn/gtwqhyjizu.html


<!-- 参考信息 -->