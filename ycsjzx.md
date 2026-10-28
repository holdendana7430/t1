代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.vqdsnc.cn/gtmlwpleyl.html

[Q28] 求和与平均
来源：http://hz.shzxlz.cn/gtngyinjuv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yuanzhike.top/gttlhqfqog.html

[Q29] 最大最小值
来源：http://hz.chenjidiqi.icu/gtuddrqrqv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.daria6918.cn/gtfvxosphs.html

[Q30] 分组统计
来源：http://hz.xuanzx.com/gtnnqemheo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gaohongyu789.top/gtqnteciou.html

[Q31] 分组后过滤
来源：http://hz.guowangkeji.top/gtnxdxniqt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cucudq.cn/gtzxdqkcrv.html

[Q32] 分组拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gthnyaypnv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.52xcode.cn/gtjlnzqokl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.316326.xyz/gtnixckwia.html

[Q33] 多列分组
来源：http://hz.gotoacloud.top/gtziglresx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yongpay.top/gtydluegvv.html

[Q34] 每组取第一条
来源：http://hz.bjfxy.top/gtacdmxsub.html

SELECT * FROM (
来源：http://hz.ydjk.org.cn/gtyxaqzcmg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenzaomai.com/gtxwccfctj.html

) t WHERE rn = 1;
来源：http://hz.quarkkingdee.top/gtnnhmianu.html

[Q35] 内连接
来源：http://hz.jqgfzy.top/gtdcvgixjn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gogol.net.cn/gtczcpuxmj.html

[Q36] 左连接
来源：http://hz.hfpthk.cn/gtzdowgrwp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinyuanbaomall.cn/gtuyftljoe.html

[Q37] 右连接
来源：http://hz.redwolf501.top/gtulvtvkdp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.316326.xyz/gtkznopdee.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jlsjyb.cn/gticavvopx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinghuilouyu.cn/gtqnvmmdqd.html

[Q39] 自连接（查上下级）
来源：http://hz.sweek.top/gtuxpskbgb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhijiandao.cn/gtyndotfah.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.fzhhl.top/gttijhoraw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xziqi.cn/gtrsbfvuly.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shangyingyoupin.top/gtknoyiorj.html

[Q41] 多表连接
来源：http://hz.fzhhl.top/gthntdhznh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zycfv.cn/gteidyjeru.html

JOIN users u ON u.id = o.user_id
来源：http://hz.0kj1m.cn/gtwhidwpzu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.birdmap.top/gtoazkasts.html

[Q42] 连接条件附加过滤
来源：http://hz.cheryme.top/gtbznwgltu.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gogol.net.cn/gtivxapuos.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.redwolf501.top/gtbmextiyo.html

[Q43] 标量子查询
来源：http://hz.gotoacloud.top/gtknatfwsj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jqgfzy.top/gtxpbbejgq.html

[Q44] IN 子查询
来源：http://hz.yuanzhike.top/gtamvoheoo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.dianchejie.cn/gthgqacjbb.html

[Q45] EXISTS 判断存在
来源：http://hz.zhongyouzk.top/gtjsoysuwd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.52xcode.cn/gtmqczwzyq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gogol.net.cn/gtbaxykwzd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yangfankeji.com/gtpqotrooh.html

[Q47] 与平均值比较
来源：http://hz.shzxlz.cn/gtpolecwvy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hywenlv.cn/gtfifmokdh.html

[Q48] CTE 公用表表达式
来源：http://hz.cucudq.cn/gtyqnaynhj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.smart0.xyz/gtgzdawnwd.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cashguo.top/gtyjunqndq.html

[Q49] 更新单行
来源：http://hz.gotoacloud.top/gtdnttkfpw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenlongwang.top/gtgjqjsegg.html

[Q50] 批量更新
来源：http://hz.quarkkingdee.top/gtgjkgteqv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.smart0.xyz/gtgepcvsra.html

[Q51] 用子查询更新
来源：http://hz.sxryk.cn/gtabmqdoaa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cheryme.top/gthqnjpnjw.html

[Q52] 删除指定行
来源：http://hz.jlsjyb.cn/gtrlqtqdlg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jyoumei.cn/gtzqafnaal.html

[Q53] 按条件删除
来源：http://hz.zhijiandao.cn/gtupoddnud.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hammf.cn/gtibhsebgx.html

[Q54] 清空表
来源：http://hz.yueranfly.top/gtayrahvgq.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigufen.top/gtrtaafhxm.html

[Q55] 排名（并列占位）
来源：http://hz.hnqzz.top/gtynfbjhxf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.wangshuangyany.cn/gtamvfgarw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jyoumei.cn/gtkeqkpffy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.chenjidiqi.icu/gtyxxfzwvk.html

[Q57] 行号
来源：http://hz.ivvv.top/gtmqasmewk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.c1oappe.top/gthdqmjrwo.html

[Q58] 累计求和
来源：http://hz.xuetiantiany.cn/gtrfqlrgqm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.fengsongda.top/gteyorxnqx.html

[Q59] 分组内累计
来源：http://hz.xziqi.cn/gtdsqnfkky.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj202588.top/gtlmxxdtnu.html

[Q60] 取上一行 / 下一行
来源：http://hz.c1oappe.top/gtzkbxfqlg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.iojbl.cn/gthmporynm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhoulong.xyz/gtexgfbnoe.html

[Q61] 移动平均
来源：http://hz.meibo888.top/gttxipvjio.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cheryme.top/gtuooxugoe.html

[Q62] 分组占比
来源：http://hz.sysykeji.top/gtlajwcncg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtudeyyxzj.html

[Q63] 开启事务
来源：http://hz.yangfankeji.com/gtmetinuiw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yvedp.cn/gtewymdkme.html

[Q64] 提交事务
来源：http://hz.vqdsnc.cn/gtdpqmyarh.html

COMMIT;
来源：http://hz.meibo888.top/gtuginoxyj.html

[Q65] 回滚事务
来源：http://hz.ywan-chungtsiang.top/gtmpkymmmx.html

ROLLBACK;
来源：http://hz.jiagoushi.top/gtyvsrtsfy.html

[Q66] 行锁查询
来源：http://hz.xingfuxueyuan.xyz/gtcjisjsys.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhiwuduotai.top/gtfqudnabz.html

[Q67] 设置隔离级别
来源：http://hz.chenzaomai.com/gtljibhzfb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.chenzaomai.com/gtxzeznmim.html

[Q68] 保存点
来源：http://hz.0kj1m.cn/gtpyswtgnz.html

SAVEPOINT sp1;
来源：http://hz.gogol.net.cn/gtiqelupgk.html

ROLLBACK TO sp1;
来源：http://hz.sweek.top/gtcutzyqza.html

[Q69] 查看执行计划
来源：http://hz.jinghuilouyu.cn/gtpjjxtfmt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yanxiufei.cn/gtnewnsqmh.html

[Q70] 更新统计信息
来源：http://hz.guowangkeji.top/gtvmedzsng.html

ANALYZE TABLE users;
来源：http://hz.haohaochexian.top/gtudmrhlvz.html

[Q71] 查看建表语句
来源：http://hz.cucudq.cn/gtfiaubpxr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhengqikj.top/gtsopqmeii.html

[Q72] 查看索引
来源：http://hz.zhijiandao.cn/gtrksreayj.html

SHOW INDEX FROM users;
来源：http://hz.ywan-chungtsiang.top/gtlyqqrjfl.html

[Q73] 查看表状态
来源：http://hz.yonumen.top/gtmdeohiwn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.tian-w.cn/gtidbcitrr.html

[Q74] 强制使用索引
来源：http://hz.hfpthk.cn/gtyvsftgho.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.52xcode.cn/gtqtxlftod.html

[Q75] 日期格式化
来源：http://hz.jqgfzy.top/gtetuvgylw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.bjfxy.top/gteywzgafy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.gaohongyu789.top/gtppzllpfz.html

[Q76] 按天统计
来源：http://hz.9152youxi.cn/gtefrgdbxj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.c1oappe.top/gtnmgtdhcg.html

[Q77] 时间加减
来源：http://hz.bjfxy.top/gtrgmocuqt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.aizwys.cn/gtaapinwju.html

[Q78] 当前时间
来源：http://hz.smart0.xyz/gtgbloxmga.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.snrcjt.cn/gtxdceuotk.html

[Q79] 字符串拼接
来源：http://hz.ydjk.org.cn/gtafyovmpk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.aizwys.cn/gtswuvkexk.html

[Q80] 字符串截取
来源：http://hz.0kj1m.cn/gtsofubswu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhijiandao.cn/gtwupkzltn.html

[Q81] 字符串替换
来源：http://hz.zhaomingkeji.xyz/gtgvwavjbk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yj20258.top/gtcijltffp.html

[Q82] 字符长度与字节长度
来源：http://hz.nanxinkj.top/gtqxnubpys.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtnxftnzyy.html

[Q83] 大小写转换
来源：http://hz.hnqzz.top/gtmhfwzywl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtswexqnjy.html

[Q84] 去除首尾空格
来源：http://hz.guannengcc.top/gtnuevehxo.html

SELECT TRIM(name) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtwtzvdsff.html

[Q85] 数值取整
来源：http://hz.xuetiantiany.cn/gtdtynyskx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.meibo888.top/gtocyzlmrx.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigufen.top/gtivqelzez.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhiwuduotai.top/gtlfxaiskv.html

[Q87] JSON 字段做条件
来源：http://hz.nanxinkj.top/gtimfzbpwt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinghuilouyu.cn/gtnafrbaga.html

[Q88] 行转列（条件聚合）
来源：http://hz.ehwqpu.com/gtcpwyselp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gaohongyu789.top/gtktqkkbll.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jqgfzy.top/gtdfpscsou.html

[Q89] 判断表是否存在
来源：http://hz.yuxming.cn/gtfzefbuvu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.chenlongwang.top/gtonffjteq.html

[Q90] 生成序号列
来源：http://hz.svipenyu.cn/gtrlqqfrzk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.fzhhl.top/gtcrkybrmb.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtqdqcxcal.html

R. Bash 专题
来源：http://hz.zycfv.cn/gtdaafecoa.html

================================================================================
来源：http://hz.guowangkeji.top/gtuvhknalb.html

[R01] shebang 与严格模式
来源：http://hz.ywan-chungtsiang.top/gtbnaomgdj.html

#!/usr/bin/env bash
来源：http://hz.zhoulong.xyz/gtajmjnmyd.html

set -euo pipefail
来源：http://hz.birdmap.top/gtwjprxymi.html

[R02] 变量赋值与使用
来源：http://hz.shzxlz.cn/gtndwsukck.html

name="Tom"; echo "$name"
来源：http://hz.jianghu66.top/gtqgogtyjg.html

[R03] 只读变量
来源：http://hz.yj20258888.top/gtcwvlmusr.html

readonly PI=3.14
来源：http://hz.nwbrower.top/gtlmcamqes.html

[R04] 位置参数
来源：http://hz.ydzc1.top/gtgcyjhqbv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ydjk.org.cn/gtzpykrsxe.html

[R05] 参数默认值
来源：http://hz.zycfv.cn/gtmzxldfvi.html

name="${1:-default}"
来源：http://hz.birdmap.top/gtmzfxkdcp.html

[R06] 判断命令是否存在
来源：http://hz.andypj.xyz/gtkontcfpm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hongshengwenyu.top/gtqjuwfrqv.html

[R07] if 判断文件
来源：http://hz.zhixingplan.top/gtdwrpibay.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tianlin.xyz/gtcbwzamoe.html

[R08] 数值比较
来源：http://hz.ywan-chungtsiang.top/gtywczohhn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shangyingyoupin.top/gtwtxrojjx.html

[R09] 字符串比较
来源：http://hz.c1oappe.top/gtytuvnimd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.bjfxy.top/gtjmppfhyt.html

[R10] 正则匹配
来源：http://hz.gotoacloud.top/gtopssmfie.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xylfe.cn/gtwvbhibaw.html

[R11] case 多分支
来源：http://hz.jlsjyb.cn/gtcimfwrfw.html

case "$1" in
来源：http://hz.jinyuanbaomall.cn/gtgwwytebd.html

start) echo "启动" ;;
来源：http://hz.snrcjt.cn/gtvxarskwx.html

stop)  echo "停止" ;;
来源：http://hz.redwolf501.top/gtwlgbusls.html

*)     echo "未知命令" ;;
来源：http://hz.aizwys.cn/gtwipvlcir.html

esac
来源：http://hz.ybcxt.top/gtcvalaejz.html

[R12] for 遍历文件
来源：http://hz.zhixingplan.top/gtacartxuj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.guowangkeji.top/gtlzepclvd.html

[R13] for 计数循环
来源：http://hz.hfpthk.cn/gtdyzbtkoa.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tanke756.top/gtxbquuyyg.html

[R14] C 风格 for
来源：http://hz.zhijiandao.cn/gtyhhiqhqm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.quarkkingdee.top/gtcdiwchxw.html

[R15] while 逐行读文件
来源：http://hz.yuanzhike.top/gtfaorgsky.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj20258.top/gtgedeqhlz.html

[R16] until 等待条件
来源：http://hz.nanxinkj.top/gtqrteegzd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.wangdashe.top/gtexzaljsa.html

[R17] 数组定义与取值
来源：http://hz.yj20258.top/gtlnvuoaih.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.feifeiyinyue.top/gtimkxtqas.html

[R18] 遍历数组
来源：http://hz.zycfv.cn/gtjsvyucww.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.chenlongwang.top/gtsgppzpvp.html

[R19] 数组长度
来源：http://hz.pengpengdd.cyou/gtramofjud.html

echo "${#arr[@]}"
来源：http://hz.hnqzz.top/gtsunfpokr.html

[R20] 关联数组（字典）
来源：http://hz.pengpengdd.cyou/gtmrpfkqbg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.smart0.xyz/gtirvijlze.html

[R21] 字符串长度
来源：http://hz.yueranfly.top/gtjtpvdhng.html

echo "${#s}"
来源：http://hz.svipenyu.cn/gtxjyctwrt.html

[R22] 截取子串
来源：http://hz.shangyingyoupin.top/gtkbdoxfpt.html

echo "${s:0:5}"
来源：http://hz.jqgufenzy.top/gtuhxeudpk.html

[R23] 字符串替换
来源：http://hz.cheryme.top/gtksrtfkxj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ivvv.top/gtilbiudbd.html

[R24] 大小写转换
来源：http://hz.chenlongwang.top/gtnceukmnx.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shanyushiyangtech.top/gtxqcwclwf.html

[R25] 去后缀 / 去前缀
来源：http://hz.gotoacloud.top/gtmtnwcdlh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xinyue.icu/gthrzyrcxl.html

[R26] 命令替换
来源：http://hz.haohaochexian.top/gtruzxfsdw.html

now=$(date +%F); echo "$now"
来源：http://hz.daria6918.cn/gtmaysenjd.html

[R27] 算术展开
来源：http://hz.hysaishi.cn/gtrrshaepw.html

echo $((1 + 2 * 3))
来源：http://hz.nanxuanxn.top/gtkkkusxlh.html

[R28] 浮点运算
来源：http://hz.pycfn.com/gtclgzwtoz.html

echo "scale=2; 10/3" | bc
来源：http://hz.cucudq.cn/gtirlldihz.html

[R29] 定义函数
来源：http://hz.hnxiangtu.top/gtymxpnwum.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.52xcode.cn/gttqpbfsvm.html

[R30] 函数返回状态码
来源：http://hz.fengsongda.top/gtflhsjzid.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.daxiang520.top/gteizisnqm.html

[R31] 局部变量
来源：http://hz.hammf.cn/gtncmoucgl.html

f() { local x=1; echo "$x"; }
来源：http://hz.ivvv.top/gtedhurvjh.html

[R32] 参数个数校验
来源：http://hz.dianchejie.cn/gtpemapryl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hnxiangtu.top/gtuesgrdsi.html

[R33] 捕获错误并提示行号
来源：http://hz.ehwqpu.com/gtzscqygsw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nanxinkj.top/gtuiiulsin.html

[R34] 退出时清理
来源：http://hz.xuetiantiany.cn/gtlqqmstyg.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.iojbl.cn/gtxvhlmfzw.html

[R35] 后台执行并等待
来源：http://hz.ehwqpu.com/gttikywoxu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.9152youxi.cn/gttbjmmsjq.html

[R36] 并发执行多个任务
来源：http://hz.jinghuilouyu.cn/gtchwnuyke.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.c1oappe.top/gtxzeddxmy.html

[R37] 把输出赋给变量
来源：http://hz.xuetiantiany.cn/gtwstdgmnq.html

files=$(ls -1)
来源：http://hz.gzhubu.top/gtcdnjmxde.html

[R38] 管道串联
来源：http://hz.yueranfly.top/gtzdcxinkk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hammf.cn/gtdkkcspfv.html

[R39] 重定向标准输出与错误
来源：http://hz.cdnleiting.top/gtqpkyvspa.html

cmd > out.log 2>&1
来源：http://hz.ydjk.org.cn/gtsvxzscjw.html

[R40] 追加写日志
来源：http://hz.chenjidiqi.icu/gtfmcypjwi.html

echo "log" >> out.log
来源：http://hz.hfpthk.cn/gtwtdeafwp.html

[R41] 丢弃输出
来源：http://hz.ydjk.org.cn/gtiwolevui.html

cmd >/dev/null 2>&1
来源：http://hz.haohaochexian.top/gteqharjmo.html

[R42] 输入重定向
来源：http://hz.yanxiufei.cn/gtyhojlgsp.html

wc -l < a.txt
来源：http://hz.xuanzx.com/gtgjrfkumg.html

[R43] 按名字查找文件
来源：http://hz.sufxvd.cn/gtegbxxayg.html

find . -name "*.log" -type f
来源：http://hz.xinyue.icu/gtgvmzfjcm.html

[R44] 按修改时间查找
来源：http://hz.zhiwuduotai.top/gtkfkwhlkm.html

find . -mtime -7 -type f
来源：http://hz.haohaochexian.top/gtcoakjysb.html

[R45] 批量删除
来源：http://hz.quarkkingdee.top/gtfdpkaplv.html

find . -name "*.tmp" -delete
来源：http://hz.ppjwa.cn/gttoyussnm.html

[R46] 递归替换文件内容
来源：http://hz.shuidangran.top/gtqlfqrewf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.snrcjt.cn/gtppqpwbme.html

[R47] sed 单行替换
来源：http://hz.birdmap.top/gttxqggyyk.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jyoumei.cn/gtcxdkqkaw.html

[R48] awk 取指定列
来源：http://hz.zhijiandao.cn/gtoztonvtt.html

awk '{print $1, $3}' a.txt
来源：http://hz.jyoumei.cn/gtzfsackkh.html

[R49] awk 带条件
来源：http://hz.jinqigufen.top/gtbqrvdwxm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ehwqpu.com/gtfwkavpbf.html

[R50] awk 求和
来源：http://hz.yvedp.cn/gtqrmgxevc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.daria6918.cn/gtjlbcqyvl.html

[R51] 排序去重取前几
来源：http://hz.nanxuanxn.top/gtqqjivqlu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yuxming.cn/gtdunkzage.html

[R52] 统计行数
来源：http://hz.xinyue.icu/gtxfrdsrsu.html

wc -l a.txt
来源：http://hz.ivvv.top/gtnlmbgnah.html

[R53] 查看文件头与实时尾
来源：http://hz.jqgufenzy.top/gtmgedaexf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dianchejie.cn/gtbsmglqsi.html

[R54] 比较两个文件
来源：http://hz.ppjwa.cn/gtciolqkmo.html

diff a.txt b.txt
来源：http://hz.nwbrower.top/gtfjwgigqa.html

[R55] 压缩与解压
来源：http://hz.yueranfly.top/gtcupvtlmy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shuidangran.top/gtlfnpodzu.html

[R56] 远程拷贝
来源：http://hz.redwolf501.top/gtomxujxhg.html

scp file user@host:/path/
来源：http://hz.svipenyu.cn/gtiboytxnp.html

[R57] 远程执行命令
来源：http://hz.guannengcc.top/gtqglhuiqi.html

ssh user@host 'uptime'
来源：http://hz.ydzc1.top/gtwqkvwqdz.html

[R58] 下载文件
来源：http://hz.wangdashe.top/gtrexevoxk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhengqikj.top/gtcmwclsyh.html

[R59] 发 POST JSON
来源：http://hz.hongshengwenyu.top/gtkwiueofq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.andypj.xyz/gtgwvkveiv.html

[R60] 只看 HTTP 状态码
来源：http://hz.yanxiufei.cn/gtnhzuovyk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhiwuduotai.top/gtsxufbgmj.html

[R61] 磁盘占用
来源：http://hz.shanyushiyangtech.top/gtpxbvlgcd.html

df -h;  du -sh *
来源：http://hz.jyoumei.cn/gtveysivus.html

[R62] 找最占空间的文件
来源：http://hz.feifeiyinyue.top/gtdjhqkgan.html

du -ah . | sort -rh | head -10
来源：http://hz.zdqjudy.top/gtwwktclac.html

[R63] 内存与进程
来源：http://hz.jinyuanbaomall.cn/gtkpmekdzo.html

free -h;  ps aux | grep nginx
来源：http://hz.jinqigufen.top/gtsrmtpipt.html

[R64] 结束进程
来源：http://hz.feifeiyinyue.top/gtfvqyeofi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.andypj.xyz/gtpgagvvdd.html

[R65] 查看端口占用
来源：http://hz.cucudq.cn/gtcpszpqku.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhoulong.xyz/gtgjbziobp.html

[R66] 定时任务
来源：http://hz.ybcxt.top/gtslidokqd.html

crontab -e;  crontab -l
来源：http://hz.guannengcc.top/gtkxotsqcc.html

[R67] 生成随机十六进制串
来源：http://hz.wangdashe.top/gtbcioqjaf.html

openssl rand -hex 16
来源：http://hz.sxryk.cn/gtrynhcfxv.html

[R68] 计算文件校验值
来源：http://hz.hnxiangtu.top/gtkeunkjas.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.wangdashe.top/gtfjxihuny.html

[R69] 生成随机密码
来源：http://hz.zycfv.cn/gtpozxstwm.html

head -c 16 /dev/urandom | base64
来源：http://hz.yonumen.top/gtxoklnuys.html

[R70] 时间戳与互转
来源：http://hz.snrcjt.cn/gtnooboafs.html

date +%s;  date -d @1700000000
来源：http://hz.nanxinkj.top/gtgjacspqx.html

[R71] 日期格式化
来源：http://hz.havefunace.top/gtzmjqgkup.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hammf.cn/gtyupeurxx.html

[R72] 等待端口就绪
来源：http://hz.yueranfly.top/gtuejvivhv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.tanke756.top/gtfxcwtxnj.html

[R73] 分割大日志
来源：http://hz.cucudq.cn/gtmxunywqx.html

split -l 1000 big.log part_
来源：http://hz.bjfxy.top/gtkdcacdmm.html

[R74] 批量重命名
来源：http://hz.jlsjyb.cn/gteujqmnzr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenlongwang.top/gtjirfrucm.html

[R75] 导出环境变量
来源：http://hz.sweek.top/gtabeqrcuz.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hongshengwenyu.top/gtucelscgp.html

[R76] 使用临时文件
来源：http://hz.yangfankeji.com/gtzffepntv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhiwuduotai.top/gtvoynjazt.html

[R77] 读取用户输入
来源：http://hz.guannengcc.top/gtjixfiwvt.html


<!-- 参考信息 -->