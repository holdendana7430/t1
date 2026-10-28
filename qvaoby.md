代发 wailian999

[Q33] 多列分组
来源：http://hz.ywan-chungtsiang.top/gtdzvrofaa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.pengpengdd.cyou/gtiktdvmes.html

[Q34] 每组取第一条
来源：http://hz.chenzaomai.com/gttmguncfb.html

SELECT * FROM (
来源：http://hz.yj20258888.top/gtnygvctok.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.bjfxy.top/gtubnyzmao.html

) t WHERE rn = 1;
来源：http://hz.tanke756.top/gtjuyuchht.html

[Q35] 内连接
来源：http://hz.hysaishi.cn/gtraffzknw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shzxlz.cn/gtwumjywai.html

[Q36] 左连接
来源：http://hz.dianchejie.cn/gtnwcznllr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenjidiqi.icu/gtwfxltsxs.html

[Q37] 右连接
来源：http://hz.vqdsnc.cn/gtokueruiv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yuxming.cn/gtoyoywcic.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jianghu66.top/gtdlqhwaja.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gogol.net.cn/gtsuziwvfz.html

[Q39] 自连接（查上下级）
来源：http://hz.jinyuanbaomall.cn/gtnurmuizf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.wangdashe.top/gtwaetkvql.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jianghu66.top/gtpspcwfyc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhaomingkeji.xyz/gtihmcdpwu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenjidiqi.icu/gtflddpntg.html

[Q41] 多表连接
来源：http://hz.mhx1999.top/gticzpvpuk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nanxinkj.top/gtemvsurgo.html

JOIN users u ON u.id = o.user_id
来源：http://hz.wangshuangyany.cn/gtsrwviows.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhongyouzk.top/gtmdibhhwp.html

[Q42] 连接条件附加过滤
来源：http://hz.gzhubu.top/gtskgepnkb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinghuilouyu.cn/gtkvflkdyk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhengqikj.top/gtiquavxtp.html

[Q43] 标量子查询
来源：http://hz.316326.xyz/gtkvcebvzh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sxryk.cn/gttfuoiyag.html

[Q44] IN 子查询
来源：http://hz.fzhhl.top/gtsiwqceke.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.9152youxi.cn/gtdcfmjxbw.html

[Q45] EXISTS 判断存在
来源：http://hz.jlsjyb.cn/gtjgcfflrq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dashuyun.cn/gtmprntfed.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gogol.net.cn/gtgrtmbcxt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jlsjyb.cn/gttndusndu.html

[Q47] 与平均值比较
来源：http://hz.hnxiangtu.top/gtgcuursob.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gaohongyu789.top/gtkjuxolor.html

[Q48] CTE 公用表表达式
来源：http://hz.havefunace.top/gtfazxozdk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.aizwys.cn/gtvxviuhbf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cdnleiting.top/gtahsbfogp.html

[Q49] 更新单行
来源：http://hz.yonumen.top/gtgwytovxg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xingfuxueyuan.xyz/gtnsudrhho.html

[Q50] 批量更新
来源：http://hz.smart0.xyz/gtarlgodww.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.daria6918.cn/gtkrhgjkbg.html

[Q51] 用子查询更新
来源：http://hz.shangyingyoupin.top/gtjobbpgkz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yj202588.top/gtaxqtkwrl.html

[Q52] 删除指定行
来源：http://hz.yuxming.cn/gtepdhhabl.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhoulong.xyz/gtjigmtfaw.html

[Q53] 按条件删除
来源：http://hz.9152youxi.cn/gtwyhojkwd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gzhubu.top/gtqcolatfr.html

[Q54] 清空表
来源：http://hz.hammf.cn/gtqgfyiydt.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigfzy.top/gtkuonogqu.html

[Q55] 排名（并列占位）
来源：http://hz.daria6918.cn/gtsbseaybm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.chenzaomai.com/gtqfismygm.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhixingplan.top/gtadpnykft.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jinyuanbaomall.cn/gturiwocfd.html

[Q57] 行号
来源：http://hz.redwolf501.top/gtmhtryuax.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hysaishi.cn/gtxbrshnji.html

[Q58] 累计求和
来源：http://hz.hfpthk.cn/gtgpgsdblj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yj202588.top/gtqhmyfskw.html

[Q59] 分组内累计
来源：http://hz.birdmap.top/gteaaalmlj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cheryme.top/gtaoqzyhnf.html

[Q60] 取上一行 / 下一行
来源：http://hz.ppjwa.cn/gtlqaluxuy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jyoumei.cn/gtjszreqex.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tanke756.top/gtwxjxrqvs.html

[Q61] 移动平均
来源：http://hz.cheryme.top/gthlefpjub.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yuanzhike.top/gtxsbcmdwy.html

[Q62] 分组占比
来源：http://hz.xuanzx.com/gtwngeeucq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.dashuyun.cn/gtxczutevj.html

[Q63] 开启事务
来源：http://hz.cqqwz.cn/gtaroyefhx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.redwolf501.top/gtawvxuxef.html

[Q64] 提交事务
来源：http://hz.ywan-chungtsiang.top/gteskirixo.html

COMMIT;
来源：http://hz.xuanzx.com/gtdjswimxl.html

[Q65] 回滚事务
来源：http://hz.daria6918.cn/gtcyvfokbj.html

ROLLBACK;
来源：http://hz.xinyue.icu/gtacpuhllj.html

[Q66] 行锁查询
来源：http://hz.zhongyouzk.top/gtmrbdkyxw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gaohongyu789.top/gthnitnaaf.html

[Q67] 设置隔离级别
来源：http://hz.ydjk.org.cn/gtuwrqipzm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinghuilouyu.cn/gtassfjppl.html

[Q68] 保存点
来源：http://hz.zycfv.cn/gttlzkpefi.html

SAVEPOINT sp1;
来源：http://hz.jlsjyb.cn/gtcbqaphep.html

ROLLBACK TO sp1;
来源：http://hz.ppjwa.cn/gtnorbelnw.html

[Q69] 查看执行计划
来源：http://hz.iojbl.cn/gtryaahjnu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinqigufen.top/gtuosyjdbl.html

[Q70] 更新统计信息
来源：http://hz.shanyushiyangkeji.top/gtckixlqdd.html

ANALYZE TABLE users;
来源：http://hz.xuanzx.com/gtsylnxwvs.html

[Q71] 查看建表语句
来源：http://hz.zhixingplan.top/gtjmheejix.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shanyushiyangtech.top/gtrwwemfjs.html

[Q72] 查看索引
来源：http://hz.xuetiantiany.cn/gtzmzjfsqw.html

SHOW INDEX FROM users;
来源：http://hz.meibo888.top/gtjcgnqcph.html

[Q73] 查看表状态
来源：http://hz.shangyingyoupin.top/gtvcdwnqqe.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhoulong.xyz/gtljbqcerr.html

[Q74] 强制使用索引
来源：http://hz.hongshengwenyu.top/gtyhgazbqd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.redwolf501.top/gteuqetzsa.html

[Q75] 日期格式化
来源：http://hz.svipenyu.cn/gtipyohbaf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.tianlin.xyz/gttsxlkcca.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sysykeji.top/gtsiakhper.html

[Q76] 按天统计
来源：http://hz.jqgufenzy.top/gtfccgelbd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sufxvd.cn/gtxhcquhry.html

[Q77] 时间加减
来源：http://hz.hnxiangtu.top/gtpheasmgm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.guannengcc.top/gtkybhqmpi.html

[Q78] 当前时间
来源：http://hz.zhoulong.xyz/gtxpwwobjh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jyoumei.cn/gtkuxvfcen.html

[Q79] 字符串拼接
来源：http://hz.shanyushiyangtech.top/gtcapsdxwa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ydjk.org.cn/gtptifbtmw.html

[Q80] 字符串截取
来源：http://hz.jqgufenzy.top/gtccprkffb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ivvv.top/gtgwyujrhu.html

[Q81] 字符串替换
来源：http://hz.shanyushiyangtech.top/gtmddxhjok.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ywan-chungtsiang.top/gtvjpmklec.html

[Q82] 字符长度与字节长度
来源：http://hz.ehwqpu.com/gtelzmfszh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.pengpengdd.cyou/gtivkejdwq.html

[Q83] 大小写转换
来源：http://hz.quarkkingdee.top/gttkdevdbm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nanxinkj.top/gtzzhohvmd.html

[Q84] 去除首尾空格
来源：http://hz.xuanzx.com/gtrczabtst.html

SELECT TRIM(name) FROM users;
来源：http://hz.cashguo.top/gtmbvvdmed.html

[Q85] 数值取整
来源：http://hz.0kj1m.cn/gtkhlzxkdy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cqqwz.cn/gtdijgovtd.html

[Q86] 读取 JSON 字段
来源：http://hz.bjfxy.top/gtxmhlbaau.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.316326.xyz/gttwiiakgu.html

[Q87] JSON 字段做条件
来源：http://hz.ybcxt.top/gtmjvnnsec.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.pycfn.com/gtwpqdzbge.html

[Q88] 行转列（条件聚合）
来源：http://hz.yj202588.top/gthnzijajd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cdnleiting.top/gtvjruyvhf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.wangdashe.top/gtxmnacmgh.html

[Q89] 判断表是否存在
来源：http://hz.hnqzz.top/gtryonepsz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhiwuduotai.top/gtwysmogbb.html

[Q90] 生成序号列
来源：http://hz.feifeiyinyue.top/gtvtcjcdhj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.mhx1999.top/gtevlagkzf.html

================================================================================
来源：http://hz.xziqi.cn/gtsobjiiyb.html

R. Bash 专题
来源：http://hz.nwbrower.top/gtpgidtlwd.html

================================================================================
来源：http://hz.guannengcc.top/gthwkwotjr.html

[R01] shebang 与严格模式
来源：http://hz.andypj.xyz/gtispeyvsd.html

#!/usr/bin/env bash
来源：http://hz.c1oappe.top/gtkyhojpil.html

set -euo pipefail
来源：http://hz.sufxvd.cn/gtxgbzfkir.html

[R02] 变量赋值与使用
来源：http://hz.xinyue.icu/gtssqogkzv.html

name="Tom"; echo "$name"
来源：http://hz.tian-w.cn/gtsfmypwbg.html

[R03] 只读变量
来源：http://hz.316326.xyz/gtygfzicos.html

readonly PI=3.14
来源：http://hz.hongshengwenyu.top/gtdqtszikh.html

[R04] 位置参数
来源：http://hz.havefunace.top/gtjzxhoqfp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhoulong.xyz/gtqusnpcgw.html

[R05] 参数默认值
来源：http://hz.hfpthk.cn/gteqdanpaw.html

name="${1:-default}"
来源：http://hz.jinqigufen.top/gtjayqushx.html

[R06] 判断命令是否存在
来源：http://hz.sweek.top/gtadqgotjs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cashguo.top/gtqmofwruc.html

[R07] if 判断文件
来源：http://hz.yongpay.top/gtnaghuucl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.aizwys.cn/gtlnxzzwea.html

[R08] 数值比较
来源：http://hz.ehwqpu.com/gtmkpznbql.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinyuanbaomall.cn/gttthwolnm.html

[R09] 字符串比较
来源：http://hz.bjfxy.top/gtuxyvyuit.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xziqi.cn/gthfuhrexz.html

[R10] 正则匹配
来源：http://hz.daxiang520.top/gtvlnhcjra.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhiwuduotai.top/gtuwisdagv.html

[R11] case 多分支
来源：http://hz.daxiang520.top/gtvqeohsyg.html

case "$1" in
来源：http://hz.9152youxi.cn/gtqvdedbjf.html

start) echo "启动" ;;
来源：http://hz.yj20258.top/gtjpqjioso.html

stop)  echo "停止" ;;
来源：http://hz.hammf.cn/gtksthssrr.html

*)     echo "未知命令" ;;
来源：http://hz.yj20258.top/gthoyefsjd.html

esac
来源：http://hz.zhijiandao.cn/gtozrmoymn.html

[R12] for 遍历文件
来源：http://hz.xinyue.icu/gtxsbmglvn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.wangdashe.top/gtidayyady.html

[R13] for 计数循环
来源：http://hz.yueranfly.top/gtfummcofb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.aibaodan.cn/gtyithpiyt.html

[R14] C 风格 for
来源：http://hz.shzxlz.cn/gtiuhcscay.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.andypj.xyz/gtrgnuhvav.html

[R15] while 逐行读文件
来源：http://hz.jyoumei.cn/gtfojfkahf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yangfankeji.com/gtwmodmbvx.html

[R16] until 等待条件
来源：http://hz.xuetiantiany.cn/gtoecfdwra.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nanxinkj.top/gtnrqfyyvq.html

[R17] 数组定义与取值
来源：http://hz.ydzc1.top/gtotzgoyfy.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hammf.cn/gtwcuwxwdb.html

[R18] 遍历数组
来源：http://hz.pengpengdd.cyou/gtggeebheb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhijiandao.cn/gtghxtczqb.html

[R19] 数组长度
来源：http://hz.jlsjyb.cn/gtvmesesqr.html

echo "${#arr[@]}"
来源：http://hz.zhongyouzk.top/gtakhxwlvy.html

[R20] 关联数组（字典）
来源：http://hz.yongpay.top/gtnqioiblm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.daxiang520.top/gtejzcpcmb.html

[R21] 字符串长度
来源：http://hz.wangshuangyany.cn/gtkfkozvuj.html

echo "${#s}"
来源：http://hz.yongpay.top/gtishvsokt.html

[R22] 截取子串
来源：http://hz.hywenlv.cn/gtyivhsmsk.html

echo "${s:0:5}"
来源：http://hz.cheryme.top/gtlewxdnzf.html

[R23] 字符串替换
来源：http://hz.hfpthk.cn/gtzwaanoym.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgufenzy.top/gtcryjvswl.html

[R24] 大小写转换
来源：http://hz.hfpthk.cn/gtzzgyfquk.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.fzhhl.top/gtzfpjjrga.html

[R25] 去后缀 / 去前缀
来源：http://hz.daria6918.cn/gteokuzquo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yvedp.cn/gtxrpsvuhw.html

[R26] 命令替换
来源：http://hz.nanxinkj.top/gtowyplfea.html

now=$(date +%F); echo "$now"
来源：http://hz.zycfv.cn/gtearpedsu.html

[R27] 算术展开
来源：http://hz.52xcode.cn/gtudkktjbs.html

echo $((1 + 2 * 3))
来源：http://hz.mhx1999.top/gtlwmghqzg.html

[R28] 浮点运算
来源：http://hz.vqdsnc.cn/gtmywdxsyv.html

echo "scale=2; 10/3" | bc
来源：http://hz.yuxming.cn/gttrmfvitm.html

[R29] 定义函数
来源：http://hz.sysykeji.top/gthovbtjag.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.fzhhl.top/gtlweblbri.html

[R30] 函数返回状态码
来源：http://hz.fengsongda.top/gtnzneekxr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jiagoushi.top/gtodcynado.html

[R31] 局部变量
来源：http://hz.yanxiufei.cn/gtcskyuzua.html

f() { local x=1; echo "$x"; }
来源：http://hz.hammf.cn/gtwiqtvncv.html

[R32] 参数个数校验
来源：http://hz.xingfuxueyuan.xyz/gtarubomfx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.tanke756.top/gtvkespyuj.html

[R33] 捕获错误并提示行号
来源：http://hz.jinghuilouyu.cn/gtfntppmsw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gaohongyu789.top/gtaqvfbdlr.html

[R34] 退出时清理
来源：http://hz.gotoacloud.top/gtpgwyxujc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gttfcpspvl.html

[R35] 后台执行并等待
来源：http://hz.ivvv.top/gtabszasoe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhaomingkeji.xyz/gtviybsidw.html

[R36] 并发执行多个任务
来源：http://hz.jianghu66.top/gtxcguxypk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ppjwa.cn/gtfiiafgfy.html

[R37] 把输出赋给变量
来源：http://hz.yvedp.cn/gtpluvcist.html

files=$(ls -1)
来源：http://hz.pengpengdd.cyou/gtibadjvcv.html

[R38] 管道串联
来源：http://hz.jinqigufen.top/gtrxaugavr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tanke756.top/gtnylczeet.html

[R39] 重定向标准输出与错误
来源：http://hz.xinyue.icu/gtflphhfme.html

cmd > out.log 2>&1
来源：http://hz.shuidangran.top/gtktoaltcd.html

[R40] 追加写日志
来源：http://hz.cqqwz.cn/gtolmetshz.html

echo "log" >> out.log
来源：http://hz.bjfxy.top/gtbpleactc.html

[R41] 丢弃输出
来源：http://hz.cheryme.top/gtyxquxuzz.html

cmd >/dev/null 2>&1
来源：http://hz.yj20258.top/gtzjxlsusl.html

[R42] 输入重定向
来源：http://hz.yueranfly.top/gtbfypyopv.html

wc -l < a.txt
来源：http://hz.svipenyu.cn/gtldrdjoiy.html

[R43] 按名字查找文件
来源：http://hz.redwolf501.top/gtvqppqbef.html

find . -name "*.log" -type f
来源：http://hz.pycfn.com/gtysbnjnzo.html

[R44] 按修改时间查找
来源：http://hz.cashguo.top/gtzueboyrl.html

find . -mtime -7 -type f
来源：http://hz.tianlin.xyz/gtdkoapfli.html

[R45] 批量删除
来源：http://hz.nanxuanxn.top/gttxmlbhou.html

find . -name "*.tmp" -delete
来源：http://hz.gzhubu.top/gtpphcsywk.html

[R46] 递归替换文件内容
来源：http://hz.pengpengdd.cyou/gtppsgrgtm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.daxiang520.top/gtfezjjuez.html

[R47] sed 单行替换
来源：http://hz.yueranfly.top/gtjylzfnoq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sufxvd.cn/gtjqpokauj.html

[R48] awk 取指定列
来源：http://hz.shuidangran.top/gtojlfnnpe.html

awk '{print $1, $3}' a.txt
来源：http://hz.xylfe.cn/gtbsgznzsh.html

[R49] awk 带条件
来源：http://hz.hammf.cn/gthrkjndhx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ppjwa.cn/gtnzpwypnn.html

[R50] awk 求和
来源：http://hz.xziqi.cn/gtmwfmemvk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.redwolf501.top/gtndbzmmps.html

[R51] 排序去重取前几
来源：http://hz.aizwys.cn/gtshdxoilt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenjidiqi.icu/gtjdqmuutn.html

[R52] 统计行数
来源：http://hz.cqqwz.cn/gtqtufodly.html

wc -l a.txt
来源：http://hz.iojbl.cn/gtbgvfzimv.html

[R53] 查看文件头与实时尾
来源：http://hz.gzhubu.top/gtavrvxvpz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinqigfzy.top/gtlogwojor.html

[R54] 比较两个文件
来源：http://hz.andypj.xyz/gthuskjguz.html

diff a.txt b.txt
来源：http://hz.sweek.top/gtiryiliym.html

[R55] 压缩与解压
来源：http://hz.316326.xyz/gtfkhakarg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yueranfly.top/gtvcgjfqwn.html

[R56] 远程拷贝
来源：http://hz.guowangkeji.top/gtvtxccucz.html

scp file user@host:/path/
来源：http://hz.jiagoushi.top/gtrmwqupte.html

[R57] 远程执行命令
来源：http://hz.xinyue.icu/gtswhmzcoc.html

ssh user@host 'uptime'
来源：http://hz.iojbl.cn/gtkurvfmzc.html

[R58] 下载文件
来源：http://hz.feifeiyinyue.top/gtysinkqiv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shzxlz.cn/gtpytwkpuw.html

[R59] 发 POST JSON
来源：http://hz.yonumen.top/gtpxlchpex.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hongshengwenyu.top/gtjmbfueri.html

[R60] 只看 HTTP 状态码
来源：http://hz.feifeiyinyue.top/gtwyzzzekc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinyuanbaomall.cn/gtjcmlvutv.html

[R61] 磁盘占用
来源：http://hz.yanxiufei.cn/gtafgvdvuw.html

df -h;  du -sh *
来源：http://hz.xuanzx.com/gtrjmrqfyt.html

[R62] 找最占空间的文件
来源：http://hz.9152youxi.cn/gtebmklprt.html

du -ah . | sort -rh | head -10
来源：http://hz.daxiang520.top/gtnvdrnsjn.html

[R63] 内存与进程
来源：http://hz.hongshengwenyu.top/gtbnqilzta.html

free -h;  ps aux | grep nginx
来源：http://hz.shanyushiyangkeji.top/gtgrvdgvdy.html

[R64] 结束进程
来源：http://hz.fengsongda.top/gtokfqxaan.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cheryme.top/gtwvgzolwa.html

[R65] 查看端口占用
来源：http://hz.tianlin.xyz/gtdjtxscwg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.fzhhl.top/gtiiiivozm.html

[R66] 定时任务
来源：http://hz.hnqzz.top/gtmhrrkyrp.html

crontab -e;  crontab -l
来源：http://hz.zhongyouzk.top/gtfcjpzxkm.html

[R67] 生成随机十六进制串
来源：http://hz.yuxming.cn/gtnbewvhvw.html

openssl rand -hex 16
来源：http://hz.andypj.xyz/gtjzvdmyki.html

[R68] 计算文件校验值
来源：http://hz.birdmap.top/gtpneqnuon.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yonumen.top/gtkjrdwxxf.html

[R69] 生成随机密码
来源：http://hz.shanyushiyangkeji.top/gtqpxyenkh.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhijiandao.cn/gtljedpspo.html

[R70] 时间戳与互转
来源：http://hz.svipenyu.cn/gtepfvblzo.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258.top/gteienfgxc.html

[R71] 日期格式化
来源：http://hz.sweek.top/gtjtkrucdq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinqigfzy.top/gtkqmppkio.html

[R72] 等待端口就绪
来源：http://hz.zhoulong.xyz/gtqghcfwmk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.guowangkeji.top/gtyemrnncy.html

[R73] 分割大日志
来源：http://hz.quarkkingdee.top/gtziaanxlz.html

split -l 1000 big.log part_
来源：http://hz.chenjidiqi.icu/gtshitiuiw.html

[R74] 批量重命名
来源：http://hz.zhoulong.xyz/gtxpinwhmn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tanke756.top/gtyputfhon.html

[R75] 导出环境变量
来源：http://hz.smart0.xyz/gtzlfpaoby.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cqqwz.cn/gtzhgyluub.html

[R76] 使用临时文件
来源：http://hz.zhongyouzk.top/gthxepsyyn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xinyue.icu/gtujwwrcwd.html

[R77] 读取用户输入
来源：http://hz.hfpthk.cn/gtevizlvki.html

read -rp "请输入: " ans
来源：http://hz.9152youxi.cn/gtmepoluzv.html

[R78] 交互式菜单
来源：http://hz.shanyushiyangtech.top/gtcuhclekq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yongpay.top/gtsexapuuq.html

[R79] 解析命令行选项
来源：http://hz.tanke756.top/gtpkmcisut.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gaohongyu789.top/gtawyakcho.html

[R80] 查看脚本执行耗时
来源：http://hz.ydjk.org.cn/gtntdszwao.html

time ./run.sh
来源：http://hz.shanyushiyangkeji.top/gtjgulrkmi.html

================================================================================
来源：http://hz.guowangkeji.top/gtdtwldwml.html

S. C / C++ 专题
来源：http://hz.haohaochexian.top/gtyrmvtwwe.html

================================================================================
来源：http://hz.jinqigufen.top/gtdiuiinwz.html

[S01] C：Hello World
来源：http://hz.jiagoushi.top/gtmiqyriok.html

#include <stdio.h>
来源：http://hz.xylfe.cn/gtdycanscm.html


<!-- 参考信息 -->