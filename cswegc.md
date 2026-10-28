代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.vqdsnc.cn/gtzhyvuxep.html

[Q22] 排序
来源：http://hz.guowangkeji.top/gtxmbcgrje.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.daxiang520.top/gtdllburzi.html

[Q23] 分页
来源：http://hz.sufxvd.cn/gtsoizkuvf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xuanzx.com/gtblmmlimr.html

[Q24] 去重
来源：http://hz.feifeiyinyue.top/gtpmzsczqb.html

SELECT DISTINCT city FROM users;
来源：http://hz.aizwys.cn/gthopcomoo.html

[Q25] 只取前 N 条
来源：http://hz.shanyushiyangtech.top/gtbesjljxx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yvedp.cn/gtijmpijgj.html

[Q26] 计数
来源：http://hz.guannengcc.top/gthxxijtlf.html

SELECT COUNT(*) FROM users;
来源：http://hz.hnqzz.top/gtvooylvpc.html

[Q27] 条件计数
来源：http://hz.wangshuangyany.cn/gttttcbwdh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jiagoushi.top/gtmdguqltx.html

[Q28] 求和与平均
来源：http://hz.hnxiangtu.top/gtycwmvdru.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zycfv.cn/gtdgnawqoi.html

[Q29] 最大最小值
来源：http://hz.wangdashe.top/gtjgkkjbrg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.aibaodan.cn/gtxdqzesej.html

[Q30] 分组统计
来源：http://hz.fengsongda.top/gtoyleugig.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shzxlz.cn/gtbuwmvbux.html

[Q31] 分组后过滤
来源：http://hz.chenjidiqi.icu/gtockogsnn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.havefunace.top/gtzfzbioia.html

[Q32] 分组拼接字符串
来源：http://hz.smart0.xyz/gtkohhaidv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jyoumei.cn/gtudsxcxib.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gaohongyu789.top/gtxcslvqhd.html

[Q33] 多列分组
来源：http://hz.mhx1999.top/gtlsdkfxls.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hysaishi.cn/gtpfzbhgoh.html

[Q34] 每组取第一条
来源：http://hz.jinqigfzy.top/gtsxayotfy.html

SELECT * FROM (
来源：http://hz.xinyue.icu/gtohpnmvzb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnxiangtu.top/gtkruwshdo.html

) t WHERE rn = 1;
来源：http://hz.daxiang520.top/gtxyfgmsyl.html

[Q35] 内连接
来源：http://hz.tianlin.xyz/gtshxxosgu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhongyouzk.top/gtzexvuzbf.html

[Q36] 左连接
来源：http://hz.xuetiantiany.cn/gtuuwvwxyf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tian-w.cn/gttqcnlozd.html

[Q37] 右连接
来源：http://hz.guowangkeji.top/gtuvsesgdr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.svipenyu.cn/gtmdmmtwdt.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhixingplan.top/gtdvsarobx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenjidiqi.icu/gtoazgifdg.html

[Q39] 自连接（查上下级）
来源：http://hz.smart0.xyz/gtagtjndiv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jianghu66.top/gtempxtusn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.havefunace.top/gtkschqmpb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinyuanbaomall.cn/gtyhzwhhxw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sxryk.cn/gteumzlqdl.html

[Q41] 多表连接
来源：http://hz.ybcxt.top/gtdjlvpwgx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinqigfzy.top/gtelmdijsr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.aizwys.cn/gtfxdlivox.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.mhx1999.top/gtqrxprdlv.html

[Q42] 连接条件附加过滤
来源：http://hz.havefunace.top/gtbfgdsvrl.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zycfv.cn/gtmqhugvrd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhongyouzk.top/gtqktlifor.html

[Q43] 标量子查询
来源：http://hz.hfpthk.cn/gtjvwnfdnp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.chenzaomai.com/gtivoiojxk.html

[Q44] IN 子查询
来源：http://hz.0kj1m.cn/gtgixazzxl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.chenzaomai.com/gtlmhluybr.html

[Q45] EXISTS 判断存在
来源：http://hz.zhaomingkeji.xyz/gttwkvrboe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shzxlz.cn/gthbsurorb.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.chenjidiqi.icu/gtnfiqvcwj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hfpthk.cn/gtxqqxvxdu.html

[Q47] 与平均值比较
来源：http://hz.gaohongyu789.top/gtvqzacise.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hnqzz.top/gtvdutgdio.html

[Q48] CTE 公用表表达式
来源：http://hz.pycfn.com/gtoecmudcr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.pycfn.com/gthemiaekc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yuxming.cn/gtlpgfpmln.html

[Q49] 更新单行
来源：http://hz.yj202588.top/gttwfgsqqw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.pengpengdd.cyou/gtjhcvmnbs.html

[Q50] 批量更新
来源：http://hz.gzhubu.top/gtcjmecfxw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.guannengcc.top/gtjwnkfngd.html

[Q51] 用子查询更新
来源：http://hz.birdmap.top/gtjveczvfa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhijiandao.cn/gtmyxdclaa.html

[Q52] 删除指定行
来源：http://hz.316326.xyz/gtetpgihrx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cqqwz.cn/gttnbhrjue.html

[Q53] 按条件删除
来源：http://hz.hnxiangtu.top/gtrddzmdzb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ywan-chungtsiang.top/gtmxsixbwq.html

[Q54] 清空表
来源：http://hz.jiagoushi.top/gtngrxeznb.html

TRUNCATE TABLE logs;
来源：http://hz.aizwys.cn/gtifgbytau.html

[Q55] 排名（并列占位）
来源：http://hz.daria6918.cn/gtkmmuytes.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xingfuxueyuan.xyz/gtymmhnerz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.daxiang520.top/gtofuhadsb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cashguo.top/gtfrrpobdw.html

[Q57] 行号
来源：http://hz.yvedp.cn/gtddhgmapg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.iojbl.cn/gtziwpqilw.html

[Q58] 累计求和
来源：http://hz.zhijiandao.cn/gtvtijbqoc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.pycfn.com/gtnkwyymuj.html

[Q59] 分组内累计
来源：http://hz.jqgfzy.top/gtcxfvbhcr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nanxuanxn.top/gtyupqvuux.html

[Q60] 取上一行 / 下一行
来源：http://hz.xuetiantiany.cn/gtbbgyiysh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.havefunace.top/gtepdjenex.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jyoumei.cn/gtjkezfdgv.html

[Q61] 移动平均
来源：http://hz.meibo888.top/gtlosqqypt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.wangshuangyany.cn/gtipuaehwz.html

[Q62] 分组占比
来源：http://hz.shangyingyoupin.top/gtdxarkmll.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtoeylufqs.html

[Q63] 开启事务
来源：http://hz.cdnleiting.top/gtpspargwu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ydzc1.top/gtlhoedhmv.html

[Q64] 提交事务
来源：http://hz.yj202588.top/gtdkdpgubg.html

COMMIT;
来源：http://hz.yj20258888.top/gtfjntgsdm.html

[Q65] 回滚事务
来源：http://hz.xinyue.icu/gtoudxjgjj.html

ROLLBACK;
来源：http://hz.0kj1m.cn/gtamtriicl.html

[Q66] 行锁查询
来源：http://hz.zhoulong.xyz/gtqmuxwdhb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shzxlz.cn/gtyhluxcwn.html

[Q67] 设置隔离级别
来源：http://hz.shangyingyoupin.top/gtumwyyitu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.svipenyu.cn/gtdqrfwrgy.html

[Q68] 保存点
来源：http://hz.feifeiyinyue.top/gtntidyjer.html

SAVEPOINT sp1;
来源：http://hz.chenlongwang.top/gtkszdiqdk.html

ROLLBACK TO sp1;
来源：http://hz.fengsongda.top/gtdqznowkl.html

[Q69] 查看执行计划
来源：http://hz.chenzaomai.com/gtkvnjliif.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sweek.top/gtiyspwhfo.html

[Q70] 更新统计信息
来源：http://hz.yuanzhike.top/gtjgvcacqy.html

ANALYZE TABLE users;
来源：http://hz.hongshengwenyu.top/gtnuqphzwq.html

[Q71] 查看建表语句
来源：http://hz.zhongyouzk.top/gtrrhjrsgl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinyuanbaomall.cn/gtjobpsxmt.html

[Q72] 查看索引
来源：http://hz.daria6918.cn/gtrxhjxcpy.html

SHOW INDEX FROM users;
来源：http://hz.jiagoushi.top/gtqsmoltqw.html

[Q73] 查看表状态
来源：http://hz.xingfuxueyuan.xyz/gtzdahzafd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cheryme.top/gtdzgsnlpm.html

[Q74] 强制使用索引
来源：http://hz.ivvv.top/gthpnhcewx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhixingplan.top/gthkpflabi.html

[Q75] 日期格式化
来源：http://hz.sysykeji.top/gtamwxwzsx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cdnleiting.top/gtertejxdn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.bjfxy.top/gtrvnnrwhq.html

[Q76] 按天统计
来源：http://hz.xuetiantiany.cn/gtmajbpjaz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hnxiangtu.top/gtyenrbvak.html

[Q77] 时间加减
来源：http://hz.zhengqikj.top/gtlpcahovw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shuidangran.top/gtuczgawjf.html

[Q78] 当前时间
来源：http://hz.cqqwz.cn/gtrcrzefwk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.mhx1999.top/gtalepawrt.html

[Q79] 字符串拼接
来源：http://hz.52xcode.cn/gtjwazajiz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hfpthk.cn/gtqwarfhsr.html

[Q80] 字符串截取
来源：http://hz.gotoacloud.top/gtbznlrjjj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.svipenyu.cn/gtsrhkpvif.html

[Q81] 字符串替换
来源：http://hz.bjfxy.top/gtgholfwzd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydjk.org.cn/gtlrdboela.html

[Q82] 字符长度与字节长度
来源：http://hz.zhixingplan.top/gtzqincnhq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.0kj1m.cn/gtecwwpxzf.html

[Q83] 大小写转换
来源：http://hz.52xcode.cn/gttnwmefjk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cdnleiting.top/gtbxpnnual.html

[Q84] 去除首尾空格
来源：http://hz.9152youxi.cn/gttjoceikv.html

SELECT TRIM(name) FROM users;
来源：http://hz.chenjidiqi.icu/gtsukrbgui.html

[Q85] 数值取整
来源：http://hz.tianlin.xyz/gtdjkztfio.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.redwolf501.top/gtxiajghjv.html

[Q86] 读取 JSON 字段
来源：http://hz.jinghuilouyu.cn/gtoxisjdwg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hywenlv.cn/gtckkjgbwu.html

[Q87] JSON 字段做条件
来源：http://hz.jinqigfzy.top/gtvqxdlqzu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ppjwa.cn/gtrkbvznce.html

[Q88] 行转列（条件聚合）
来源：http://hz.xingfuxueyuan.xyz/gtvdbbgnle.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hammf.cn/gtkqafltsv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hammf.cn/gtzbtyebjc.html

[Q89] 判断表是否存在
来源：http://hz.sufxvd.cn/gtnolmzxlo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.havefunace.top/gtaaiumnxu.html

[Q90] 生成序号列
来源：http://hz.yvedp.cn/gtgwtyxpyz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yuxming.cn/gtjdodikij.html

================================================================================
来源：http://hz.yanxiufei.cn/gtapueyipq.html

R. Bash 专题
来源：http://hz.xylfe.cn/gtbxnpfqty.html

================================================================================
来源：http://hz.daxiang520.top/gtgvwtguac.html

[R01] shebang 与严格模式
来源：http://hz.feifeiyinyue.top/gtweelklrs.html

#!/usr/bin/env bash
来源：http://hz.fengsongda.top/gtdxavjvey.html

set -euo pipefail
来源：http://hz.cheryme.top/gtetzynwnm.html

[R02] 变量赋值与使用
来源：http://hz.yj20258.top/gtlqpsbjtu.html

name="Tom"; echo "$name"
来源：http://hz.shanyushiyangkeji.top/gtlxeingae.html

[R03] 只读变量
来源：http://hz.sxryk.cn/gtrufeldni.html

readonly PI=3.14
来源：http://hz.mhx1999.top/gtfsgrqjpn.html

[R04] 位置参数
来源：http://hz.havefunace.top/gtaieuivzb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinyuanbaomall.cn/gtplvpjfan.html

[R05] 参数默认值
来源：http://hz.fengsongda.top/gtbvnqygxo.html

name="${1:-default}"
来源：http://hz.dashuyun.cn/gtchurspap.html

[R06] 判断命令是否存在
来源：http://hz.yonumen.top/gtilyvuvmj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenlongwang.top/gtkdvulwzl.html

[R07] if 判断文件
来源：http://hz.wangdashe.top/gtvvafncag.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jyoumei.cn/gtymeqsjly.html

[R08] 数值比较
来源：http://hz.zhixingplan.top/gtdofoqdft.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.pengpengdd.cyou/gtjwbtsfks.html

[R09] 字符串比较
来源：http://hz.ydzc1.top/gtqxxwspti.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.feifeiyinyue.top/gtnzmhyhhj.html

[R10] 正则匹配
来源：http://hz.hnxiangtu.top/gttrkznvyq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinqigufen.top/gtnoxihlsm.html

[R11] case 多分支
来源：http://hz.wangdashe.top/gtmgrduyuw.html

case "$1" in
来源：http://hz.tanke756.top/gtppcfdpvw.html

start) echo "启动" ;;
来源：http://hz.yueranfly.top/gtxchkokzh.html

stop)  echo "停止" ;;
来源：http://hz.meibo888.top/gtxdcqznqy.html

*)     echo "未知命令" ;;
来源：http://hz.yj20258888.top/gtqxgasdek.html

esac
来源：http://hz.feifeiyinyue.top/gteumrwunr.html

[R12] for 遍历文件
来源：http://hz.shzxlz.cn/gtwcppcjkv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.daxiang520.top/gtqvkjulem.html

[R13] for 计数循环
来源：http://hz.pycfn.com/gtsmgyrobe.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hammf.cn/gtummfsveb.html

[R14] C 风格 for
来源：http://hz.hnxiangtu.top/gtwzocwhzr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zdqjudy.top/gtisxqoxdb.html

[R15] while 逐行读文件
来源：http://hz.xziqi.cn/gtbhgwcbrz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yongpay.top/gtmtflqxrk.html

[R16] until 等待条件
来源：http://hz.ydzc1.top/gtnjveqczm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.pycfn.com/gtksyatsvx.html

[R17] 数组定义与取值
来源：http://hz.jinqigufen.top/gtvusjnkif.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sufxvd.cn/gtoaekvyhb.html

[R18] 遍历数组
来源：http://hz.smart0.xyz/gthvkngkka.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.guannengcc.top/gtqqggogor.html

[R19] 数组长度
来源：http://hz.redwolf501.top/gtqoxufltw.html

echo "${#arr[@]}"
来源：http://hz.ywan-chungtsiang.top/gtoqtlmfmj.html

[R20] 关联数组（字典）
来源：http://hz.quarkkingdee.top/gtpehhfgek.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cdnleiting.top/gteoyxtlif.html

[R21] 字符串长度
来源：http://hz.dianchejie.cn/gttgquubgc.html

echo "${#s}"
来源：http://hz.chenlongwang.top/gtvctmscti.html

[R22] 截取子串
来源：http://hz.yueranfly.top/gtunyggalj.html

echo "${s:0:5}"
来源：http://hz.yueranfly.top/gtucmutrjo.html

[R23] 字符串替换
来源：http://hz.316326.xyz/gtvukbkmwt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ywan-chungtsiang.top/gtzdaqroaq.html

[R24] 大小写转换
来源：http://hz.pycfn.com/gtgkqadmdx.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhiwuduotai.top/gtndwwswmq.html

[R25] 去后缀 / 去前缀
来源：http://hz.snrcjt.cn/gtdedtfgpq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xinyue.icu/gtpxbbralm.html

[R26] 命令替换
来源：http://hz.nwbrower.top/gtulsdwtie.html

now=$(date +%F); echo "$now"
来源：http://hz.zhongyouzk.top/gtjjdsrlik.html

[R27] 算术展开
来源：http://hz.zhixingplan.top/gtnpnaajbm.html

echo $((1 + 2 * 3))
来源：http://hz.ydzc1.top/gtddnjuiut.html

[R28] 浮点运算
来源：http://hz.nanxinkj.top/gtmjqeqfom.html

echo "scale=2; 10/3" | bc
来源：http://hz.tianlin.xyz/gtkzwjmice.html

[R29] 定义函数
来源：http://hz.hnxiangtu.top/gteaeoziwh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gaohongyu789.top/gthcjymhwj.html

[R30] 函数返回状态码
来源：http://hz.chenjidiqi.icu/gtavxqsnwe.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.tian-w.cn/gtyhposdbt.html

[R31] 局部变量
来源：http://hz.gzhubu.top/gturtvfehq.html

f() { local x=1; echo "$x"; }
来源：http://hz.hammf.cn/gtyaetdwjq.html

[R32] 参数个数校验
来源：http://hz.zhongyouzk.top/gtlrxucjek.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.kuanghao11.cn/gtplgzcgid.html

[R33] 捕获错误并提示行号
来源：http://hz.ydjk.org.cn/gthctwnxcn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xuanzx.com/gtykciokxq.html

[R34] 退出时清理
来源：http://hz.zhijiandao.cn/gtfybmndwm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hfpthk.cn/gtlttszfiw.html

[R35] 后台执行并等待
来源：http://hz.ywan-chungtsiang.top/gtrqtbfubk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.birdmap.top/gtcrrdymvr.html

[R36] 并发执行多个任务
来源：http://hz.ywan-chungtsiang.top/gtrdrjhkku.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xziqi.cn/gtfdxauvhw.html

[R37] 把输出赋给变量
来源：http://hz.ybcxt.top/gtwmxzjpbd.html

files=$(ls -1)
来源：http://hz.xuanzx.com/gttobmdfcu.html

[R38] 管道串联
来源：http://hz.xylfe.cn/gtezqolddz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hfpthk.cn/gtubphobro.html

[R39] 重定向标准输出与错误
来源：http://hz.jianghu66.top/gtyusbyikj.html

cmd > out.log 2>&1
来源：http://hz.chenzaomai.com/gtewvcrtez.html

[R40] 追加写日志
来源：http://hz.jinyuanbaomall.cn/gttjzstiua.html

echo "log" >> out.log
来源：http://hz.jinyuanbaomall.cn/gtdvukbkbb.html

[R41] 丢弃输出
来源：http://hz.sweek.top/gtthxywcok.html

cmd >/dev/null 2>&1
来源：http://hz.shanyushiyangkeji.top/gtyvafktkn.html

[R42] 输入重定向
来源：http://hz.birdmap.top/gtezmzqlvt.html

wc -l < a.txt
来源：http://hz.tianlin.xyz/gtnzommzpw.html

[R43] 按名字查找文件
来源：http://hz.chenzaomai.com/gtcnzfufpp.html

find . -name "*.log" -type f
来源：http://hz.jinqigfzy.top/gtiucoshmr.html

[R44] 按修改时间查找
来源：http://hz.gaohongyu789.top/gtrsekfulk.html

find . -mtime -7 -type f
来源：http://hz.daria6918.cn/gtixgrgfef.html

[R45] 批量删除
来源：http://hz.shuidangran.top/gtnyrwtqrj.html

find . -name "*.tmp" -delete
来源：http://hz.wangshuangyany.cn/gtaixwhvcl.html

[R46] 递归替换文件内容
来源：http://hz.nanxinkj.top/gtzxrhlnef.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hnqzz.top/gtarxkaumz.html

[R47] sed 单行替换
来源：http://hz.guowangkeji.top/gtmuqbvnvw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shzxlz.cn/gtsvtjdaqk.html

[R48] awk 取指定列
来源：http://hz.mhx1999.top/gtgbtpbtrj.html

awk '{print $1, $3}' a.txt
来源：http://hz.hnqzz.top/gtytrntnww.html

[R49] awk 带条件
来源：http://hz.wangdashe.top/gtmofjdtos.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shangyingyoupin.top/gtghzrgotm.html

[R50] awk 求和
来源：http://hz.cheryme.top/gtgxyhkaqo.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jianghu66.top/gtvxgnsewm.html

[R51] 排序去重取前几
来源：http://hz.yanxiufei.cn/gthkchjvqb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jyoumei.cn/gtkjzowwbp.html

[R52] 统计行数
来源：http://hz.chenjidiqi.icu/gtetjfviao.html

wc -l a.txt
来源：http://hz.chenzaomai.com/gtryxdtdgo.html

[R53] 查看文件头与实时尾
来源：http://hz.cashguo.top/gtyilfxyaj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.mhx1999.top/gtyeixiyii.html

[R54] 比较两个文件
来源：http://hz.yangfankeji.com/gtsgrrzppy.html

diff a.txt b.txt
来源：http://hz.aizwys.cn/gtcobimtto.html

[R55] 压缩与解压
来源：http://hz.shanyushiyangtech.top/gtzfpypttf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.havefunace.top/gttbhddopf.html

[R56] 远程拷贝
来源：http://hz.xziqi.cn/gtykvhfcdl.html

scp file user@host:/path/
来源：http://hz.jinqigfzy.top/gtvkpqyamx.html

[R57] 远程执行命令
来源：http://hz.jiagoushi.top/gtifbnhpjw.html

ssh user@host 'uptime'
来源：http://hz.dianchejie.cn/gtrxgqldtc.html

[R58] 下载文件
来源：http://hz.tianlin.xyz/gtjvjqtdfm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xylfe.cn/gtovvidpqb.html

[R59] 发 POST JSON
来源：http://hz.gzhubu.top/gtnadtggnv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yongpay.top/gtkbcdpoun.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinqigfzy.top/gtkfwcdjde.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shanyushiyangkeji.top/gtdqlgraof.html

[R61] 磁盘占用
来源：http://hz.guowangkeji.top/gtqgfgzglx.html

df -h;  du -sh *
来源：http://hz.chenlongwang.top/gtrvnykdpp.html

[R62] 找最占空间的文件
来源：http://hz.gogol.net.cn/gtmtezgpth.html

du -ah . | sort -rh | head -10
来源：http://hz.zhoulong.xyz/gtxypszekh.html

[R63] 内存与进程
来源：http://hz.yj20258.top/gtpabdnhij.html

free -h;  ps aux | grep nginx
来源：http://hz.sysykeji.top/gtyxatfmmq.html

[R64] 结束进程
来源：http://hz.jiagoushi.top/gtfaewdyiw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xingfuxueyuan.xyz/gtasibfgel.html

[R65] 查看端口占用
来源：http://hz.vqdsnc.cn/gtiklxsdyq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hammf.cn/gtxofpwnsy.html

[R66] 定时任务
来源：http://hz.dianchejie.cn/gtcsyonuvq.html

crontab -e;  crontab -l
来源：http://hz.zycfv.cn/gtfyhyxcyx.html

[R67] 生成随机十六进制串
来源：http://hz.cdnleiting.top/gtnbwmeuqv.html

openssl rand -hex 16
来源：http://hz.yvedp.cn/gtlyxwyhxp.html

[R68] 计算文件校验值
来源：http://hz.xingfuxueyuan.xyz/gtqylmsadw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhongyouzk.top/gtmuutcwtp.html

[R69] 生成随机密码
来源：http://hz.gogol.net.cn/gtbwbhmzwj.html

head -c 16 /dev/urandom | base64
来源：http://hz.cucudq.cn/gtadqwiokz.html

[R70] 时间戳与互转
来源：http://hz.cdnleiting.top/gtxnlcgclb.html

date +%s;  date -d @1700000000
来源：http://hz.gaohongyu789.top/gtqyzodizr.html

[R71] 日期格式化
来源：http://hz.meibo888.top/gtuaqiwmea.html


<!-- 参考信息 -->