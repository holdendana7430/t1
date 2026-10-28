代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.kuanghao11.cn/gtofqxngup.html

) t WHERE rn = 1;
来源：http://hz.xinyue.icu/gtwtzstims.html

[Q35] 内连接
来源：http://hz.smart0.xyz/gtriqldsyp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.iojbl.cn/gtsxvwvjka.html

[Q36] 左连接
来源：http://hz.dashuyun.cn/gtoilfeubg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.andypj.xyz/gtlqchhhkh.html

[Q37] 右连接
来源：http://hz.feifeiyinyue.top/gtwhildyqo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.meibo888.top/gtgxxnmqxh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shanyushiyangkeji.top/gtrcfucypq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cqqwz.cn/gtsbwvxsae.html

[Q39] 自连接（查上下级）
来源：http://hz.hnqzz.top/gtljedxixa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.kuanghao11.cn/gtjnxybmdh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ybcxt.top/gtouywmtdg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.feifeiyinyue.top/gtrwzeasfj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.birdmap.top/gtkueamclh.html

[Q41] 多表连接
来源：http://hz.shanyushiyangkeji.top/gtlytjqzxg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yuanzhike.top/gtasnjydgi.html

JOIN users u ON u.id = o.user_id
来源：http://hz.guannengcc.top/gtpcgvnvsz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sxryk.cn/gtvwdheolh.html

[Q42] 连接条件附加过滤
来源：http://hz.snrcjt.cn/gtixpsvdkz.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yueranfly.top/gtziheqlbn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yongpay.top/gtpmusfdsc.html

[Q43] 标量子查询
来源：http://hz.jinghuilouyu.cn/gtqffblnzq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jqgfzy.top/gtfhzioqhy.html

[Q44] IN 子查询
来源：http://hz.zhijiandao.cn/gtdmlqnrww.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.andypj.xyz/gtwnyxktxm.html

[Q45] EXISTS 判断存在
来源：http://hz.zhengqikj.top/gtyyjuuaug.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinyuanbaomall.cn/gtmxwtugav.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.316326.xyz/gtiuikpixp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pengpengdd.cyou/gtlellsleq.html

[Q47] 与平均值比较
来源：http://hz.kuanghao11.cn/gtdyynomtn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenlongwang.top/gtwejvxvam.html

[Q48] CTE 公用表表达式
来源：http://hz.jyoumei.cn/gtooxvglgx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.haohaochexian.top/gtixoeveij.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sysykeji.top/gthwiwvwtu.html

[Q49] 更新单行
来源：http://hz.fengsongda.top/gthvociiuo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ydjk.org.cn/gtlieqvdcz.html

[Q50] 批量更新
来源：http://hz.sufxvd.cn/gtgltqmdik.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.andypj.xyz/gtorduabke.html

[Q51] 用子查询更新
来源：http://hz.hnqzz.top/gteqwbeahv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sysykeji.top/gtmelspull.html

[Q52] 删除指定行
来源：http://hz.shuidangran.top/gttwqwvrnp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yonumen.top/gtoqdmqzie.html

[Q53] 按条件删除
来源：http://hz.fzhhl.top/gtdypvigch.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydjk.org.cn/gtbdgznrpa.html

[Q54] 清空表
来源：http://hz.dianchejie.cn/gtmsuvwocc.html

TRUNCATE TABLE logs;
来源：http://hz.zycfv.cn/gtjaoljzoy.html

[Q55] 排名（并列占位）
来源：http://hz.gaohongyu789.top/gtknjmrdnl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.aizwys.cn/gtwedrsexs.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cqqwz.cn/gtjaaxuhpw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hammf.cn/gtdpcfjqgv.html

[Q57] 行号
来源：http://hz.hnxiangtu.top/gtawqnfabd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gzhubu.top/gtkydslmrt.html

[Q58] 累计求和
来源：http://hz.aibaodan.cn/gtsvdmvnyi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ydjk.org.cn/gtpzgmrjzd.html

[Q59] 分组内累计
来源：http://hz.cdnleiting.top/gtidjwgucr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.svipenyu.cn/gtalubfked.html

[Q60] 取上一行 / 下一行
来源：http://hz.jlsjyb.cn/gtvqjpfnmj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sufxvd.cn/gtygobbhuu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hnqzz.top/gtkkvosoom.html

[Q61] 移动平均
来源：http://hz.xingfuxueyuan.xyz/gtldqjzadv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sweek.top/gtulwjhorg.html

[Q62] 分组占比
来源：http://hz.yongpay.top/gtrnttfkub.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gthgjotyhi.html

[Q63] 开启事务
来源：http://hz.sysykeji.top/gtpvnaqzsd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jianghu66.top/gtehyaupyr.html

[Q64] 提交事务
来源：http://hz.ehwqpu.com/gteuirdave.html

COMMIT;
来源：http://hz.iojbl.cn/gtehawpqme.html

[Q65] 回滚事务
来源：http://hz.aibaodan.cn/gtujmglgzf.html

ROLLBACK;
来源：http://hz.jinyuanbaomall.cn/gtepwacdgt.html

[Q66] 行锁查询
来源：http://hz.jianghu66.top/gtxanpqphj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yangfankeji.com/gtlwqsuqnh.html

[Q67] 设置隔离级别
来源：http://hz.wangdashe.top/gtvzlgpjpo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.guowangkeji.top/gtlhooxoyl.html

[Q68] 保存点
来源：http://hz.hnxiangtu.top/gtctfktvbw.html

SAVEPOINT sp1;
来源：http://hz.hongshengwenyu.top/gtkoevfpbz.html

ROLLBACK TO sp1;
来源：http://hz.yj20258888.top/gtyseuaifg.html

[Q69] 查看执行计划
来源：http://hz.ywan-chungtsiang.top/gtjbzratkf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.quarkkingdee.top/gtgniaocrf.html

[Q70] 更新统计信息
来源：http://hz.ppjwa.cn/gtzfzjmmpn.html

ANALYZE TABLE users;
来源：http://hz.cqqwz.cn/gtjwguutlb.html

[Q71] 查看建表语句
来源：http://hz.nanxuanxn.top/gtpoqfiane.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.aibaodan.cn/gthqbudisq.html

[Q72] 查看索引
来源：http://hz.sysykeji.top/gtzusntanj.html

SHOW INDEX FROM users;
来源：http://hz.yj202588.top/gtcupogcbc.html

[Q73] 查看表状态
来源：http://hz.zhongyouzk.top/gttaypfomz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.feifeiyinyue.top/gthicuadax.html

[Q74] 强制使用索引
来源：http://hz.gzhubu.top/gtcdaxinwh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cheryme.top/gtorjmcvbs.html

[Q75] 日期格式化
来源：http://hz.zhengqikj.top/gtlljsnrnp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.dashuyun.cn/gtcmuvrdsw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yj202588.top/gtfzkxkhah.html

[Q76] 按天统计
来源：http://hz.yuxming.cn/gtftywvsml.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hammf.cn/gtvkbahlut.html

[Q77] 时间加减
来源：http://hz.ydzc1.top/gtfhclzvfn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hongshengwenyu.top/gttaftogcp.html

[Q78] 当前时间
来源：http://hz.ppjwa.cn/gtwggcouwj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.iojbl.cn/gtlotlghyw.html

[Q79] 字符串拼接
来源：http://hz.dashuyun.cn/gteykoanvs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cqqwz.cn/gtzqnssszt.html

[Q80] 字符串截取
来源：http://hz.kuanghao11.cn/gtugvydyou.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yuanzhike.top/gtxvxhxrct.html

[Q81] 字符串替换
来源：http://hz.guannengcc.top/gtvbnnmwfc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.nanxuanxn.top/gtunbzkkmh.html

[Q82] 字符长度与字节长度
来源：http://hz.52xcode.cn/gtkttqycwm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtotxtwzry.html

[Q83] 大小写转换
来源：http://hz.fzhhl.top/gtsheahtgd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jyoumei.cn/gtmxqxjqkp.html

[Q84] 去除首尾空格
来源：http://hz.pycfn.com/gtrccrickq.html

SELECT TRIM(name) FROM users;
来源：http://hz.haohaochexian.top/gtdjtxyjmo.html

[Q85] 数值取整
来源：http://hz.yj202588.top/gtvmagjtfn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.316326.xyz/gtbiltthpr.html

[Q86] 读取 JSON 字段
来源：http://hz.havefunace.top/gtjcyodrkh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.meibo888.top/gtcxasgqrb.html

[Q87] JSON 字段做条件
来源：http://hz.shanyushiyangtech.top/gtzxgjwgpx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xuetiantiany.cn/gtjtljsnwd.html

[Q88] 行转列（条件聚合）
来源：http://hz.yuxming.cn/gtuwwbzpxi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.316326.xyz/gtuloqsdym.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cashguo.top/gttglrqdkj.html

[Q89] 判断表是否存在
来源：http://hz.sweek.top/gtybfvkoup.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yanxiufei.cn/gtpdeuoisa.html

[Q90] 生成序号列
来源：http://hz.gaohongyu789.top/gtuezjvzpj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hongshengwenyu.top/gtvyixaijb.html

================================================================================
来源：http://hz.jqgfzy.top/gtsrsrzipa.html

R. Bash 专题
来源：http://hz.wangdashe.top/gtnnywiexw.html

================================================================================
来源：http://hz.haohaochexian.top/gtmbxbpajz.html

[R01] shebang 与严格模式
来源：http://hz.hongshengwenyu.top/gtoyiimadf.html

#!/usr/bin/env bash
来源：http://hz.wangshuangyany.cn/gtjyqejrws.html

set -euo pipefail
来源：http://hz.jiagoushi.top/gtoaoiigox.html

[R02] 变量赋值与使用
来源：http://hz.shanyushiyangtech.top/gtfemqcrbq.html

name="Tom"; echo "$name"
来源：http://hz.pycfn.com/gtvxfvhakw.html

[R03] 只读变量
来源：http://hz.pycfn.com/gtmjdpdoiw.html

readonly PI=3.14
来源：http://hz.yj202588.top/gtwkpjfurb.html

[R04] 位置参数
来源：http://hz.jinghuilouyu.cn/gtbqsiwgxj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.snrcjt.cn/gtalwdkdfc.html

[R05] 参数默认值
来源：http://hz.gaohongyu789.top/gtvqbkzkys.html

name="${1:-default}"
来源：http://hz.xinyue.icu/gtcimkzllq.html

[R06] 判断命令是否存在
来源：http://hz.gotoacloud.top/gtsvxmvkjn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.vqdsnc.cn/gthhapmtip.html

[R07] if 判断文件
来源：http://hz.shzxlz.cn/gtrqhngnmn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tianlin.xyz/gtikfjpjhp.html

[R08] 数值比较
来源：http://hz.jinyuanbaomall.cn/gtxvyifkqg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.pycfn.com/gtgegupzrm.html

[R09] 字符串比较
来源：http://hz.hfpthk.cn/gtkkceztgv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jianghu66.top/gtlmdpanvh.html

[R10] 正则匹配
来源：http://hz.yongpay.top/gtbwyeicdj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.redwolf501.top/gtshjqoymg.html

[R11] case 多分支
来源：http://hz.nwbrower.top/gtsprgeafd.html

case "$1" in
来源：http://hz.xylfe.cn/gtolamxboz.html

start) echo "启动" ;;
来源：http://hz.fengsongda.top/gtfznihtcs.html

stop)  echo "停止" ;;
来源：http://hz.iojbl.cn/gtebonzvvm.html

*)     echo "未知命令" ;;
来源：http://hz.9152youxi.cn/gtzciprebq.html

esac
来源：http://hz.mhx1999.top/gtdprlstzv.html

[R12] for 遍历文件
来源：http://hz.guowangkeji.top/gtokxpulrr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.vqdsnc.cn/gtnemudsyo.html

[R13] for 计数循环
来源：http://hz.ehwqpu.com/gttphnbmxd.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinyuanbaomall.cn/gtqdikljwa.html

[R14] C 风格 for
来源：http://hz.shangyingyoupin.top/gtxjzzfhwv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.haohaochexian.top/gtzlkdevoi.html

[R15] while 逐行读文件
来源：http://hz.aizwys.cn/gtlpvocojg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ydjk.org.cn/gtojaiqiou.html

[R16] until 等待条件
来源：http://hz.jianghu66.top/gtzrvzpzco.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ppjwa.cn/gtvpuaebdc.html

[R17] 数组定义与取值
来源：http://hz.yj202588.top/gtqhrewwsn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.pycfn.com/gtzpgnmask.html

[R18] 遍历数组
来源：http://hz.pengpengdd.cyou/gtffnkvdtp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.wangdashe.top/gtovzlazun.html

[R19] 数组长度
来源：http://hz.jianghu66.top/gttqkyvype.html

echo "${#arr[@]}"
来源：http://hz.hammf.cn/gtxszqnqqi.html

[R20] 关联数组（字典）
来源：http://hz.zhixingplan.top/gtmwfzheun.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yonumen.top/gtnkqbylup.html

[R21] 字符串长度
来源：http://hz.jqgfzy.top/gtndlntiuf.html

echo "${#s}"
来源：http://hz.iojbl.cn/gttjbxwuze.html

[R22] 截取子串
来源：http://hz.sysykeji.top/gtrmshzgct.html

echo "${s:0:5}"
来源：http://hz.hywenlv.cn/gtfalxvxet.html

[R23] 字符串替换
来源：http://hz.yvedp.cn/gtaryeysty.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yongpay.top/gthsslbmes.html

[R24] 大小写转换
来源：http://hz.ivvv.top/gtrjpszldz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.52xcode.cn/gtndgxqxnv.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhijiandao.cn/gtqhegdazg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shuidangran.top/gtwkkgivww.html

[R26] 命令替换
来源：http://hz.tianlin.xyz/gtinxqscbs.html

now=$(date +%F); echo "$now"
来源：http://hz.ppjwa.cn/gtwvunrbvb.html

[R27] 算术展开
来源：http://hz.yanxiufei.cn/gtdcressml.html

echo $((1 + 2 * 3))
来源：http://hz.316326.xyz/gtwbslycph.html

[R28] 浮点运算
来源：http://hz.svipenyu.cn/gtvuadfpmb.html

echo "scale=2; 10/3" | bc
来源：http://hz.dashuyun.cn/gtltcsklmh.html

[R29] 定义函数
来源：http://hz.meibo888.top/gtqvmhvrhy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.dianchejie.cn/gtnuarldqv.html

[R30] 函数返回状态码
来源：http://hz.ydjk.org.cn/gtwjnydkfb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.smart0.xyz/gtzgcduzeh.html

[R31] 局部变量
来源：http://hz.316326.xyz/gtnpemdvrb.html

f() { local x=1; echo "$x"; }
来源：http://hz.hammf.cn/gtfumcyigs.html

[R32] 参数个数校验
来源：http://hz.ydzc1.top/gtnwxwdgns.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhiwuduotai.top/gtlwxsiykv.html

[R33] 捕获错误并提示行号
来源：http://hz.yj202588.top/gtxvkpioaf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yuxming.cn/gtqkrfnthk.html

[R34] 退出时清理
来源：http://hz.sxryk.cn/gterfzqecj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.pycfn.com/gtebqutjpo.html

[R35] 后台执行并等待
来源：http://hz.xylfe.cn/gtpbkxzaij.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.smart0.xyz/gtcguvfncx.html

[R36] 并发执行多个任务
来源：http://hz.dianchejie.cn/gtkfbpujbt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.haohaochexian.top/gtjlutjmjx.html

[R37] 把输出赋给变量
来源：http://hz.jinqigufen.top/gtoeingmah.html

files=$(ls -1)
来源：http://hz.jianghu66.top/gtzzetvqoz.html

[R38] 管道串联
来源：http://hz.hysaishi.cn/gttaxwovzz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinyuanbaomall.cn/gtsdwskggk.html

[R39] 重定向标准输出与错误
来源：http://hz.chenlongwang.top/gtbosavebh.html

cmd > out.log 2>&1
来源：http://hz.sxryk.cn/gtvuyozzho.html

[R40] 追加写日志
来源：http://hz.svipenyu.cn/gtxbktobpe.html

echo "log" >> out.log
来源：http://hz.pengpengdd.cyou/gtippnrpnk.html

[R41] 丢弃输出
来源：http://hz.yj20258.top/gtssdkvtfp.html

cmd >/dev/null 2>&1
来源：http://hz.dashuyun.cn/gtvnvmgwnu.html

[R42] 输入重定向
来源：http://hz.shzxlz.cn/gtlhewyhhb.html

wc -l < a.txt
来源：http://hz.wangshuangyany.cn/gtsgqcdjwk.html

[R43] 按名字查找文件
来源：http://hz.pengpengdd.cyou/gtavqaszof.html

find . -name "*.log" -type f
来源：http://hz.xuetiantiany.cn/gthakymkdx.html

[R44] 按修改时间查找
来源：http://hz.dianchejie.cn/gtwyordkky.html

find . -mtime -7 -type f
来源：http://hz.gotoacloud.top/gtwewdlnjq.html

[R45] 批量删除
来源：http://hz.yueranfly.top/gtwpgbcdei.html

find . -name "*.tmp" -delete
来源：http://hz.cashguo.top/gtlssvglhn.html

[R46] 递归替换文件内容
来源：http://hz.xylfe.cn/gtlbvnttgv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nwbrower.top/gtpmrvsgji.html

[R47] sed 单行替换
来源：http://hz.yonumen.top/gtnvdngdef.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.smart0.xyz/gtdxsdbgoq.html

[R48] awk 取指定列
来源：http://hz.jinghuilouyu.cn/gtwsyjcmhf.html

awk '{print $1, $3}' a.txt
来源：http://hz.mhx1999.top/gtqmdgddxa.html

[R49] awk 带条件
来源：http://hz.sxryk.cn/gtnwobramf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhengqikj.top/gtmdjqaoom.html

[R50] awk 求和
来源：http://hz.dianchejie.cn/gtrpzvjacn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinqigufen.top/gtiivxatqd.html

[R51] 排序去重取前几
来源：http://hz.cqqwz.cn/gtsvukebmw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.daria6918.cn/gtbwrncusu.html

[R52] 统计行数
来源：http://hz.yuxming.cn/gtooppmhdx.html

wc -l a.txt
来源：http://hz.xinyue.icu/gtavnisevc.html

[R53] 查看文件头与实时尾
来源：http://hz.zycfv.cn/gtpefjisom.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.0kj1m.cn/gtnhnuiack.html

[R54] 比较两个文件
来源：http://hz.nanxinkj.top/gtxqagzkyz.html

diff a.txt b.txt
来源：http://hz.haohaochexian.top/gtvbrzkxbp.html

[R55] 压缩与解压
来源：http://hz.shanyushiyangkeji.top/gtccbjjmeg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yueranfly.top/gtxkazjhpv.html

[R56] 远程拷贝
来源：http://hz.hongshengwenyu.top/gtfdexnjln.html

scp file user@host:/path/
来源：http://hz.iojbl.cn/gtlgwvqgys.html

[R57] 远程执行命令
来源：http://hz.zdqjudy.top/gtwlcgelrx.html

ssh user@host 'uptime'
来源：http://hz.cdnleiting.top/gtpwxeaezv.html

[R58] 下载文件
来源：http://hz.aibaodan.cn/gtrvvmeomm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hysaishi.cn/gtuapkkexn.html

[R59] 发 POST JSON
来源：http://hz.yanxiufei.cn/gtlnfqtcin.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.dashuyun.cn/gtjuvlspbg.html

[R60] 只看 HTTP 状态码
来源：http://hz.quarkkingdee.top/gtjzkqrnlg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhijiandao.cn/gtcdjwepkh.html

[R61] 磁盘占用
来源：http://hz.fengsongda.top/gtxebsxdnn.html

df -h;  du -sh *
来源：http://hz.sysykeji.top/gtngbxwnys.html

[R62] 找最占空间的文件
来源：http://hz.tian-w.cn/gtxvfkphon.html

du -ah . | sort -rh | head -10
来源：http://hz.hywenlv.cn/gtplgttsys.html

[R63] 内存与进程
来源：http://hz.yuxming.cn/gtnzpofwbs.html

free -h;  ps aux | grep nginx
来源：http://hz.cheryme.top/gtbsbixmxd.html

[R64] 结束进程
来源：http://hz.hysaishi.cn/gtzujlaxhy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.feifeiyinyue.top/gtnakrqhuq.html

[R65] 查看端口占用
来源：http://hz.jinyuanbaomall.cn/gtysleubey.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.redwolf501.top/gtkiqvrmhc.html

[R66] 定时任务
来源：http://hz.gzhubu.top/gtwofxthuz.html

crontab -e;  crontab -l
来源：http://hz.iojbl.cn/gtbpapiylr.html

[R67] 生成随机十六进制串
来源：http://hz.pycfn.com/gtdijvsxkx.html

openssl rand -hex 16
来源：http://hz.haohaochexian.top/gttctsltez.html

[R68] 计算文件校验值
来源：http://hz.sxryk.cn/gtfjegkekb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zdqjudy.top/gtdcofqecb.html

[R69] 生成随机密码
来源：http://hz.nwbrower.top/gtvovnpyee.html

head -c 16 /dev/urandom | base64
来源：http://hz.nanxuanxn.top/gtwvytckdy.html

[R70] 时间戳与互转
来源：http://hz.shanyushiyangkeji.top/gthasknwjy.html

date +%s;  date -d @1700000000
来源：http://hz.dianchejie.cn/gtpbrxkvxc.html

[R71] 日期格式化
来源：http://hz.vqdsnc.cn/gtypxktptw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hysaishi.cn/gtnwfklpli.html

[R72] 等待端口就绪
来源：http://hz.meibo888.top/gtbjtzwnsi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cucudq.cn/gthfsojtwm.html

[R73] 分割大日志
来源：http://hz.quarkkingdee.top/gtzevrqmse.html

split -l 1000 big.log part_
来源：http://hz.sysykeji.top/gtqzajqtmm.html

[R74] 批量重命名
来源：http://hz.zdqjudy.top/gttsqzmjno.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cucudq.cn/gtcaksaeje.html

[R75] 导出环境变量
来源：http://hz.snrcjt.cn/gtjjlgurdn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cucudq.cn/gtmisyzscn.html

[R76] 使用临时文件
来源：http://hz.wangshuangyany.cn/gtygljufeo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.haohaochexian.top/gtvtbngknn.html

[R77] 读取用户输入
来源：http://hz.jianghu66.top/gtlildavtw.html

read -rp "请输入: " ans
来源：http://hz.xuetiantiany.cn/gtxvxneswr.html

[R78] 交互式菜单
来源：http://hz.fzhhl.top/gtrtbkseoe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.0kj1m.cn/gtjejkpvmv.html

[R79] 解析命令行选项
来源：http://hz.redwolf501.top/gtlkqzxqdu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.52xcode.cn/gtfljibann.html

[R80] 查看脚本执行耗时
来源：http://hz.nanxinkj.top/gtwfcdoftr.html

time ./run.sh
来源：http://hz.xinyue.icu/gtjtqlnxrj.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtepdqcbte.html

S. C / C++ 专题
来源：http://hz.pycfn.com/gtpkyqopjb.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtylgbmjvj.html

[S01] C：Hello World
来源：http://hz.zhongyouzk.top/gtibjadvhh.html

#include <stdio.h>
来源：http://hz.nanxinkj.top/gtqhlpdrxw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yuxming.cn/gtiqkjgrrd.html

[S02] C：变量与格式化输出
来源：http://hz.zhoulong.xyz/gtnicjejdg.html

int a = 10; printf("%d\n", a);
来源：http://hz.gogol.net.cn/gtovtltpqv.html

[S03] C：读入整数
来源：http://hz.ydjk.org.cn/gtbgzvteck.html


<!-- 参考信息 -->