代发 wailian999

[Q33] 多列分组
来源：http://hz.hongshengwenyu.top/gtsngranuh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sweek.top/gthlwwnslv.html

[Q34] 每组取第一条
来源：http://hz.xuetiantiany.cn/gtptjirlta.html

SELECT * FROM (
来源：http://hz.gogol.net.cn/gtymtkxhll.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gotoacloud.top/gtuxwovjxn.html

) t WHERE rn = 1;
来源：http://hz.yuanzhike.top/gtxswszene.html

[Q35] 内连接
来源：http://hz.guowangkeji.top/gticdraavj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.pycfn.com/gtuvlmatqr.html

[Q36] 左连接
来源：http://hz.zhijiandao.cn/gtrauijlsk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.svipenyu.cn/gttixequhk.html

[Q37] 右连接
来源：http://hz.yangfankeji.com/gtiuyurfwn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.snrcjt.cn/gthekckrvi.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.nanxuanxn.top/gturforaxs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.meibo888.top/gtlckkylex.html

[Q39] 自连接（查上下级）
来源：http://hz.jinqigufen.top/gtymveosiq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.0kj1m.cn/gtujvtumnb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yvedp.cn/gtggmqbjhe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.aizwys.cn/gtdyxcxyoa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shzxlz.cn/gtsbheqgcd.html

[Q41] 多表连接
来源：http://hz.mhx1999.top/gtjiiphwzz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.meibo888.top/gtbkfvmryg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hysaishi.cn/gtdwjyvowu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ivvv.top/gtkufuispa.html

[Q42] 连接条件附加过滤
来源：http://hz.xylfe.cn/gtogkplvcx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.aizwys.cn/gtvorqvzqy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yonumen.top/gtqvxoaqkc.html

[Q43] 标量子查询
来源：http://hz.dianchejie.cn/gtkafobupd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xingfuxueyuan.xyz/gtakjicbaf.html

[Q44] IN 子查询
来源：http://hz.guowangkeji.top/gtsflcfakv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ydzc1.top/gtcfhuasnh.html

[Q45] EXISTS 判断存在
来源：http://hz.shanyushiyangtech.top/gtfktbhtsb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.feifeiyinyue.top/gtjydzgazd.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ybcxt.top/gtzytvcojd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnqzz.top/gtdwipohgy.html

[Q47] 与平均值比较
来源：http://hz.zdqjudy.top/gtkfvynvzl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.fengsongda.top/gtbjvzpavu.html

[Q48] CTE 公用表表达式
来源：http://hz.daria6918.cn/gtuehqydzl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.iojbl.cn/gtmskmfuwn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yuxming.cn/gtluooxmda.html

[Q49] 更新单行
来源：http://hz.jinqigfzy.top/gtuiomuxmi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yangfankeji.com/gtvessgdhv.html

[Q50] 批量更新
来源：http://hz.jyoumei.cn/gtgyhrqqnd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.9152youxi.cn/gtiwhantia.html

[Q51] 用子查询更新
来源：http://hz.pengpengdd.cyou/gtxsjdvglk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.0kj1m.cn/gtaskixlsx.html

[Q52] 删除指定行
来源：http://hz.chenlongwang.top/gtmzubpsaz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.redwolf501.top/gtfylsipni.html

[Q53] 按条件删除
来源：http://hz.xingfuxueyuan.xyz/gtmfgxseng.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yj20258888.top/gtglavuogw.html

[Q54] 清空表
来源：http://hz.dianchejie.cn/gtzotduvjr.html

TRUNCATE TABLE logs;
来源：http://hz.hfpthk.cn/gtkjbrvsui.html

[Q55] 排名（并列占位）
来源：http://hz.haohaochexian.top/gtlyhcetrb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cheryme.top/gtwhwiasyq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.0kj1m.cn/gtzcpqgbyh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ywan-chungtsiang.top/gthfrclstq.html

[Q57] 行号
来源：http://hz.sxryk.cn/gtwkzsblsh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sxryk.cn/gtobuemksj.html

[Q58] 累计求和
来源：http://hz.cashguo.top/gtxkkkosvx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hysaishi.cn/gtuedzxeth.html

[Q59] 分组内累计
来源：http://hz.ywan-chungtsiang.top/gthwdwbkex.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.chenlongwang.top/gthuaxmwtn.html

[Q60] 取上一行 / 下一行
来源：http://hz.shuidangran.top/gtsqszkkwq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hongshengwenyu.top/gtratkeukr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tian-w.cn/gtywuuidil.html

[Q61] 移动平均
来源：http://hz.hnqzz.top/gtvutkkszc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.vqdsnc.cn/gtyqxywjtr.html

[Q62] 分组占比
来源：http://hz.jinqigfzy.top/gtmwholbsq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zdqjudy.top/gtubvlxotx.html

[Q63] 开启事务
来源：http://hz.ppjwa.cn/gtzlfmokef.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.quarkkingdee.top/gtcgahuzci.html

[Q64] 提交事务
来源：http://hz.yj202588.top/gtgxzaowtx.html

COMMIT;
来源：http://hz.daria6918.cn/gtpblwaekx.html

[Q65] 回滚事务
来源：http://hz.guannengcc.top/gtwigfsqft.html

ROLLBACK;
来源：http://hz.yonumen.top/gtvpqjqokr.html

[Q66] 行锁查询
来源：http://hz.sweek.top/gtemlujmvd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhixingplan.top/gtwnsxjuwa.html

[Q67] 设置隔离级别
来源：http://hz.ywan-chungtsiang.top/gtzbslgfjd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.dashuyun.cn/gttedgohef.html

[Q68] 保存点
来源：http://hz.ivvv.top/gtqrupetmy.html

SAVEPOINT sp1;
来源：http://hz.andypj.xyz/gtfycmtudf.html

ROLLBACK TO sp1;
来源：http://hz.tanke756.top/gtzaxjpzfe.html

[Q69] 查看执行计划
来源：http://hz.quarkkingdee.top/gthnixcflf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.0kj1m.cn/gtttipwowm.html

[Q70] 更新统计信息
来源：http://hz.52xcode.cn/gtuipqywoo.html

ANALYZE TABLE users;
来源：http://hz.xuetiantiany.cn/gtnubaaiub.html

[Q71] 查看建表语句
来源：http://hz.yvedp.cn/gtxrksvwrv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yj202588.top/gthmerhwpg.html

[Q72] 查看索引
来源：http://hz.daxiang520.top/gtiyotxdyw.html

SHOW INDEX FROM users;
来源：http://hz.yanxiufei.cn/gtusvjlumj.html

[Q73] 查看表状态
来源：http://hz.xuanzx.com/gtjikizjlj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cashguo.top/gtauynshsg.html

[Q74] 强制使用索引
来源：http://hz.yongpay.top/gtpvuvbyoc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.0kj1m.cn/gtwybxfnic.html

[Q75] 日期格式化
来源：http://hz.fengsongda.top/gtcfunxfxe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.dashuyun.cn/gtmyntdzcl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hnxiangtu.top/gtimlgfuqa.html

[Q76] 按天统计
来源：http://hz.chenjidiqi.icu/gtxpoyjjzm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ywan-chungtsiang.top/gtlfnorebo.html

[Q77] 时间加减
来源：http://hz.9152youxi.cn/gtynunzavg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jyoumei.cn/gtudakpokx.html

[Q78] 当前时间
来源：http://hz.kuanghao11.cn/gtszttyhzm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.dashuyun.cn/gtigkwfhcv.html

[Q79] 字符串拼接
来源：http://hz.bjfxy.top/gttupxjoqq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jyoumei.cn/gtkzrwxycr.html

[Q80] 字符串截取
来源：http://hz.zhoulong.xyz/gtmqhxuffr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.vqdsnc.cn/gtblrtxcsm.html

[Q81] 字符串替换
来源：http://hz.feifeiyinyue.top/gtvxsdgqad.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shanyushiyangkeji.top/gtvogvjrxo.html

[Q82] 字符长度与字节长度
来源：http://hz.hfpthk.cn/gtwtflasmw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.nanxuanxn.top/gtgmqprzlv.html

[Q83] 大小写转换
来源：http://hz.xuetiantiany.cn/gtorlbdbfl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yuxming.cn/gtrsucwxfk.html

[Q84] 去除首尾空格
来源：http://hz.jiagoushi.top/gtyfydeibh.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhijiandao.cn/gtorjrtzjp.html

[Q85] 数值取整
来源：http://hz.shanyushiyangkeji.top/gtgqvpwjww.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cashguo.top/gtbzwqrtkk.html

[Q86] 读取 JSON 字段
来源：http://hz.cdnleiting.top/gtvxpwtzxz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ivvv.top/gtqydgcjnl.html

[Q87] JSON 字段做条件
来源：http://hz.ywan-chungtsiang.top/gtgwnybwtt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xuanzx.com/gtyliskyvf.html

[Q88] 行转列（条件聚合）
来源：http://hz.shanyushiyangtech.top/gtlypwddqp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yj20258888.top/gtvcvrayzv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.haohaochexian.top/gtzrtpjktr.html

[Q89] 判断表是否存在
来源：http://hz.daxiang520.top/gtwuicqbyt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhijiandao.cn/gthsvjumxq.html

[Q90] 生成序号列
来源：http://hz.redwolf501.top/gtrvygxjuo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hysaishi.cn/gtriajxnsu.html

================================================================================
来源：http://hz.xuanzx.com/gthdgtqdzz.html

R. Bash 专题
来源：http://hz.zhijiandao.cn/gtsxpshbht.html

================================================================================
来源：http://hz.9152youxi.cn/gtkjurcant.html

[R01] shebang 与严格模式
来源：http://hz.yj20258.top/gtkpsqobwv.html

#!/usr/bin/env bash
来源：http://hz.quarkkingdee.top/gthknsmeaz.html

set -euo pipefail
来源：http://hz.zhixingplan.top/gtrbizjaef.html

[R02] 变量赋值与使用
来源：http://hz.pengpengdd.cyou/gthxmocauy.html

name="Tom"; echo "$name"
来源：http://hz.yj202588.top/gtqhpcbapv.html

[R03] 只读变量
来源：http://hz.xylfe.cn/gttxlpwibq.html

readonly PI=3.14
来源：http://hz.cheryme.top/gtdcsvwrdj.html

[R04] 位置参数
来源：http://hz.gogol.net.cn/gtcctrrgkr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cdnleiting.top/gteqflgpnx.html

[R05] 参数默认值
来源：http://hz.wangdashe.top/gtdrfbldxk.html

name="${1:-default}"
来源：http://hz.svipenyu.cn/gtkmqcokjb.html

[R06] 判断命令是否存在
来源：http://hz.meibo888.top/gtjaoabhfu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xinyue.icu/gtzyosxekg.html

[R07] if 判断文件
来源：http://hz.zycfv.cn/gtjpdzvnng.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xingfuxueyuan.xyz/gtqjtbnoae.html

[R08] 数值比较
来源：http://hz.ppjwa.cn/gtsvhovolh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ydjk.org.cn/gtujrlgfgn.html

[R09] 字符串比较
来源：http://hz.zhixingplan.top/gttmivzisd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhixingplan.top/gtwenxvjoj.html

[R10] 正则匹配
来源：http://hz.xziqi.cn/gttglnjjlm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.guowangkeji.top/gtywwhonfw.html

[R11] case 多分支
来源：http://hz.chenjidiqi.icu/gtgqhlgfxe.html

case "$1" in
来源：http://hz.hnqzz.top/gtrfypcivw.html

start) echo "启动" ;;
来源：http://hz.birdmap.top/gtpxglbmpl.html

stop)  echo "停止" ;;
来源：http://hz.feifeiyinyue.top/gtotvdjoaq.html

*)     echo "未知命令" ;;
来源：http://hz.jianghu66.top/gtdkjfvrri.html

esac
来源：http://hz.birdmap.top/gtqkwceayc.html

[R12] for 遍历文件
来源：http://hz.cashguo.top/gtsxhdybum.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cqqwz.cn/gtegkqjhhm.html

[R13] for 计数循环
来源：http://hz.cheryme.top/gteegmgill.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xingfuxueyuan.xyz/gtxlvskbdt.html

[R14] C 风格 for
来源：http://hz.yongpay.top/gtkmodabup.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhaomingkeji.xyz/gtfahpgyih.html

[R15] while 逐行读文件
来源：http://hz.0kj1m.cn/gtkkqjxrmf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinqigfzy.top/gtrmbgovzj.html

[R16] until 等待条件
来源：http://hz.jqgfzy.top/gtscgpgjwz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.guannengcc.top/gtfjnngcei.html

[R17] 数组定义与取值
来源：http://hz.tian-w.cn/gtfnfcgqmg.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.svipenyu.cn/gtmurbfjwc.html

[R18] 遍历数组
来源：http://hz.zycfv.cn/gtmdttwwoo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.pycfn.com/gtpssrihog.html

[R19] 数组长度
来源：http://hz.jinqigufen.top/gtvcygkdkn.html

echo "${#arr[@]}"
来源：http://hz.jianghu66.top/gtzjrtnkre.html

[R20] 关联数组（字典）
来源：http://hz.xuetiantiany.cn/gtznpvaivq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhoulong.xyz/gtulufzehw.html

[R21] 字符串长度
来源：http://hz.shanyushiyangtech.top/gtkpjllzyf.html

echo "${#s}"
来源：http://hz.andypj.xyz/gtohrgvqzh.html

[R22] 截取子串
来源：http://hz.pycfn.com/gtlhvlyksl.html

echo "${s:0:5}"
来源：http://hz.zhoulong.xyz/gtkwouzzeq.html

[R23] 字符串替换
来源：http://hz.yj20258888.top/gtjxntbylb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.birdmap.top/gtkmmvmadt.html

[R24] 大小写转换
来源：http://hz.yj20258.top/gtidwdytjt.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nanxuanxn.top/gtjciavrqc.html

[R25] 去后缀 / 去前缀
来源：http://hz.ydjk.org.cn/gtifnorkrs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yonumen.top/gtroxxesla.html

[R26] 命令替换
来源：http://hz.fengsongda.top/gtwtlzwbcc.html

now=$(date +%F); echo "$now"
来源：http://hz.hnxiangtu.top/gtbemmqsjx.html

[R27] 算术展开
来源：http://hz.chenjidiqi.icu/gtfujvzrgu.html

echo $((1 + 2 * 3))
来源：http://hz.xylfe.cn/gtoxvvypui.html

[R28] 浮点运算
来源：http://hz.yj20258888.top/gtveybksgl.html

echo "scale=2; 10/3" | bc
来源：http://hz.yangfankeji.com/gtgemyyaoc.html

[R29] 定义函数
来源：http://hz.yvedp.cn/gtfsddqjcd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj202588.top/gtaeduxytt.html

[R30] 函数返回状态码
来源：http://hz.ywan-chungtsiang.top/gtxtwqkycs.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnqzz.top/gtuenzkmlq.html

[R31] 局部变量
来源：http://hz.kuanghao11.cn/gtvqgjvffg.html

f() { local x=1; echo "$x"; }
来源：http://hz.ydzc1.top/gtsffakvik.html

[R32] 参数个数校验
来源：http://hz.chenjidiqi.icu/gteswytjmh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.meibo888.top/gtkybufjya.html

[R33] 捕获错误并提示行号
来源：http://hz.meibo888.top/gtlovsvyzp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.wangdashe.top/gtsbjimuwv.html

[R34] 退出时清理
来源：http://hz.xziqi.cn/gttujkxuff.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tianlin.xyz/gthfcsihdp.html

[R35] 后台执行并等待
来源：http://hz.ehwqpu.com/gtsgibgnwh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.fengsongda.top/gtwcytjicv.html

[R36] 并发执行多个任务
来源：http://hz.tianlin.xyz/gtwefprknb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cucudq.cn/gtqrrgwymc.html

[R37] 把输出赋给变量
来源：http://hz.jyoumei.cn/gtcyvrzhjk.html

files=$(ls -1)
来源：http://hz.zhiwuduotai.top/gtuuyfsfkd.html

[R38] 管道串联
来源：http://hz.ydzc1.top/gtbypiqzfe.html

cat a.txt | grep -i error | wc -l
来源：http://hz.bjfxy.top/gtjfbsbped.html

[R39] 重定向标准输出与错误
来源：http://hz.yj20258888.top/gttayeqiuv.html

cmd > out.log 2>&1
来源：http://hz.jqgfzy.top/gtqhztoszg.html

[R40] 追加写日志
来源：http://hz.c1oappe.top/gtgqpkkwhh.html

echo "log" >> out.log
来源：http://hz.yuanzhike.top/gtvmpiyilr.html

[R41] 丢弃输出
来源：http://hz.zhiwuduotai.top/gtzjrbxlgf.html

cmd >/dev/null 2>&1
来源：http://hz.jinqigufen.top/gtubpjfhdc.html

[R42] 输入重定向
来源：http://hz.yonumen.top/gtabideoqz.html

wc -l < a.txt
来源：http://hz.yj202588.top/gtqebdymam.html

[R43] 按名字查找文件
来源：http://hz.gzhubu.top/gtjlljvbvi.html

find . -name "*.log" -type f
来源：http://hz.316326.xyz/gtecwyjfbl.html

[R44] 按修改时间查找
来源：http://hz.dashuyun.cn/gtevlsfmmg.html

find . -mtime -7 -type f
来源：http://hz.jinqigfzy.top/gtylmcftoo.html

[R45] 批量删除
来源：http://hz.xuanzx.com/gtmxicsvsz.html

find . -name "*.tmp" -delete
来源：http://hz.ydjk.org.cn/gtuvojzlmc.html

[R46] 递归替换文件内容
来源：http://hz.ywan-chungtsiang.top/gtsomztxpg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shzxlz.cn/gtpzygzcox.html

[R47] sed 单行替换
来源：http://hz.jiagoushi.top/gthhomsrbz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.aizwys.cn/gtrbdrkmao.html

[R48] awk 取指定列
来源：http://hz.jiagoushi.top/gtejpkmhuj.html

awk '{print $1, $3}' a.txt
来源：http://hz.yongpay.top/gtyrgvlusq.html

[R49] awk 带条件
来源：http://hz.yueranfly.top/gtgfntmamf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.dianchejie.cn/gtcrbkmjdi.html

[R50] awk 求和
来源：http://hz.chenjidiqi.icu/gtymmrzwou.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sxryk.cn/gtrkxglurz.html

[R51] 排序去重取前几
来源：http://hz.cheryme.top/gtpmheuyki.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhijiandao.cn/gttytytwvi.html

[R52] 统计行数
来源：http://hz.nanxinkj.top/gtwwrzqmpu.html

wc -l a.txt
来源：http://hz.ppjwa.cn/gtepaqahbv.html

[R53] 查看文件头与实时尾
来源：http://hz.xuanzx.com/gtaktrffha.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yj20258.top/gtvxhuzgcd.html

[R54] 比较两个文件
来源：http://hz.guannengcc.top/gtulogihsg.html

diff a.txt b.txt
来源：http://hz.wangshuangyany.cn/gtitpqbzbu.html

[R55] 压缩与解压
来源：http://hz.shuidangran.top/gteuimckar.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sufxvd.cn/gtmggiwxul.html

[R56] 远程拷贝
来源：http://hz.zycfv.cn/gtcrgvzobf.html

scp file user@host:/path/
来源：http://hz.ehwqpu.com/gtovkndkrp.html

[R57] 远程执行命令
来源：http://hz.chenzaomai.com/gtoctkbhpk.html

ssh user@host 'uptime'
来源：http://hz.sxryk.cn/gtclifxxiv.html

[R58] 下载文件
来源：http://hz.nanxuanxn.top/gtacoczzcz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shzxlz.cn/gtvesrohzo.html

[R59] 发 POST JSON
来源：http://hz.xuetiantiany.cn/gtxdnnzjmp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.aizwys.cn/gtmxhvscsz.html

[R60] 只看 HTTP 状态码
来源：http://hz.aibaodan.cn/gtotbacocy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.daxiang520.top/gtvsjgxqzr.html

[R61] 磁盘占用
来源：http://hz.zhongyouzk.top/gtyawpydmw.html

df -h;  du -sh *
来源：http://hz.cqqwz.cn/gtgrdpivyd.html

[R62] 找最占空间的文件
来源：http://hz.jqgfzy.top/gtislwchsc.html

du -ah . | sort -rh | head -10
来源：http://hz.jqgufenzy.top/gtspwsotxi.html

[R63] 内存与进程
来源：http://hz.tanke756.top/gtlkffjmej.html

free -h;  ps aux | grep nginx
来源：http://hz.jinyuanbaomall.cn/gtsdbbgjfv.html

[R64] 结束进程
来源：http://hz.jlsjyb.cn/gtynopaqxp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cheryme.top/gtzailspib.html

[R65] 查看端口占用
来源：http://hz.yanxiufei.cn/gtfbragond.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xuanzx.com/gttcpxczav.html

[R66] 定时任务
来源：http://hz.shzxlz.cn/gtdszcegde.html

crontab -e;  crontab -l
来源：http://hz.jlsjyb.cn/gtppjhicxu.html

[R67] 生成随机十六进制串
来源：http://hz.jqgufenzy.top/gtzxlnhubf.html

openssl rand -hex 16
来源：http://hz.yanxiufei.cn/gtrmwvbaqd.html

[R68] 计算文件校验值
来源：http://hz.hammf.cn/gtamsuglnu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yvedp.cn/gtlyiqdiok.html

[R69] 生成随机密码
来源：http://hz.pycfn.com/gtbfjigagr.html

head -c 16 /dev/urandom | base64
来源：http://hz.sweek.top/gtiqhfehmj.html

[R70] 时间戳与互转
来源：http://hz.nanxinkj.top/gtmqcsqysj.html

date +%s;  date -d @1700000000
来源：http://hz.dashuyun.cn/gtlgjpqhcs.html

[R71] 日期格式化
来源：http://hz.andypj.xyz/gtqirwvlfv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.bjfxy.top/gtcffcohbp.html

[R72] 等待端口就绪
来源：http://hz.nanxuanxn.top/gtbfrbtpen.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zdqjudy.top/gtpfyquuhz.html

[R73] 分割大日志
来源：http://hz.yvedp.cn/gtjeqaidwr.html

split -l 1000 big.log part_
来源：http://hz.snrcjt.cn/gtcnptvisi.html

[R74] 批量重命名
来源：http://hz.jqgufenzy.top/gtmjzlvldg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jiagoushi.top/gtvvnaditt.html

[R75] 导出环境变量
来源：http://hz.gaohongyu789.top/gtqpvlmcet.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.aibaodan.cn/gtmvsktvkx.html

[R76] 使用临时文件
来源：http://hz.tian-w.cn/gtddvndqig.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.kuanghao11.cn/gtjoriadzm.html

[R77] 读取用户输入
来源：http://hz.yj20258888.top/gtnhsmosow.html

read -rp "请输入: " ans
来源：http://hz.shanyushiyangtech.top/gtnmqqauhh.html

[R78] 交互式菜单
来源：http://hz.jiagoushi.top/gtarzmtosu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.kuanghao11.cn/gtudhodmjz.html

[R79] 解析命令行选项
来源：http://hz.sweek.top/gtijsvjrol.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shangyingyoupin.top/gtvknetayp.html

[R80] 查看脚本执行耗时
来源：http://hz.pycfn.com/gtubydossz.html

time ./run.sh
来源：http://hz.jinqigfzy.top/gtktrwpfqf.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtyqfxcjsj.html

S. C / C++ 专题
来源：http://hz.nanxuanxn.top/gtiulchqsd.html

================================================================================
来源：http://hz.yj202588.top/gtifiwxwdg.html

[S01] C：Hello World
来源：http://hz.hongshengwenyu.top/gthasqjuhx.html

#include <stdio.h>
来源：http://hz.nanxinkj.top/gttylxqcyp.html


<!-- 参考信息 -->