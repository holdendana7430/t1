代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hfpthk.cn/gtipmikgyx.html

[Q32] 分组拼接字符串
来源：http://hz.xuanzx.com/gtjhfxjlnw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gttvahayxd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nanxuanxn.top/gttbzddfvb.html

[Q33] 多列分组
来源：http://hz.zycfv.cn/gtqxagehul.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinyuanbaomall.cn/gtrndvyzlh.html

[Q34] 每组取第一条
来源：http://hz.gogol.net.cn/gtablvutaa.html

SELECT * FROM (
来源：http://hz.gzhubu.top/gtsxtwozdy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.bjfxy.top/gtqalvuitl.html

) t WHERE rn = 1;
来源：http://hz.yuanzhike.top/gtnhwwfvbs.html

[Q35] 内连接
来源：http://hz.zhoulong.xyz/gtftyxqtcs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.birdmap.top/gtdxqqeuqr.html

[Q36] 左连接
来源：http://hz.meibo888.top/gtxxvlrsui.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.birdmap.top/gtnrkpkuds.html

[Q37] 右连接
来源：http://hz.jyoumei.cn/gtjpbeknvu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.feifeiyinyue.top/gtojokecnx.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yangfankeji.com/gtpuswspxj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yangfankeji.com/gttzkqmsmz.html

[Q39] 自连接（查上下级）
来源：http://hz.yanxiufei.cn/gtpfsgzlwg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.fzhhl.top/gtsufpcktp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.chenzaomai.com/gtyxevirwt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.meibo888.top/gtpivgupsn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gotoacloud.top/gtlfwwghyl.html

[Q41] 多表连接
来源：http://hz.jinghuilouyu.cn/gtnnzlolyu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.kuanghao11.cn/gtjodvbqng.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yvedp.cn/gtsdhwwgyk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.pengpengdd.cyou/gtsflmuzlm.html

[Q42] 连接条件附加过滤
来源：http://hz.shuidangran.top/gtlyyjnqch.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hfpthk.cn/gtkclvisfv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ydjk.org.cn/gtypjhgyee.html

[Q43] 标量子查询
来源：http://hz.hammf.cn/gtcibwjvzp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hywenlv.cn/gtwzllrstl.html

[Q44] IN 子查询
来源：http://hz.zhiwuduotai.top/gtyxwlwoiz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.guowangkeji.top/gtpmvdwbry.html

[Q45] EXISTS 判断存在
来源：http://hz.ivvv.top/gtvlczfrgd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhengqikj.top/gtvmmcuycc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sxryk.cn/gthikqtwib.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.quarkkingdee.top/gtiroiycbp.html

[Q47] 与平均值比较
来源：http://hz.nanxinkj.top/gthlquhjgo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hysaishi.cn/gtpcwdowkk.html

[Q48] CTE 公用表表达式
来源：http://hz.smart0.xyz/gtxcvdazwn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jyoumei.cn/gtcpilelop.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yueranfly.top/gtplwvyeih.html

[Q49] 更新单行
来源：http://hz.tanke756.top/gtwdcuyjer.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jyoumei.cn/gtsbppdvhe.html

[Q50] 批量更新
来源：http://hz.shzxlz.cn/gtnsxdledj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yangfankeji.com/gtbqjmxnjw.html

[Q51] 用子查询更新
来源：http://hz.chenlongwang.top/gtwwirmtex.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yj20258888.top/gtbgnvdxsx.html

[Q52] 删除指定行
来源：http://hz.zhiwuduotai.top/gtrbkeokea.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yueranfly.top/gtlfrcunei.html

[Q53] 按条件删除
来源：http://hz.yueranfly.top/gtgsmonnpt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yuxming.cn/gtmbtsksxp.html

[Q54] 清空表
来源：http://hz.daxiang520.top/gtbkclgfar.html

TRUNCATE TABLE logs;
来源：http://hz.wangshuangyany.cn/gtjitbpyok.html

[Q55] 排名（并列占位）
来源：http://hz.guowangkeji.top/gtonwpyczo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.havefunace.top/gtnhvwqskg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shanyushiyangkeji.top/gthowpvgiz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.fengsongda.top/gtdoqqesjl.html

[Q57] 行号
来源：http://hz.zdqjudy.top/gtxectvstp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.quarkkingdee.top/gtzulnntsq.html

[Q58] 累计求和
来源：http://hz.mhx1999.top/gtxpfjooap.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xuanzx.com/gtxhtxqocr.html

[Q59] 分组内累计
来源：http://hz.ydzc1.top/gtvhpnovst.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yanxiufei.cn/gtgzmlqdkd.html

[Q60] 取上一行 / 下一行
来源：http://hz.vqdsnc.cn/gtwpnbbyql.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.fzhhl.top/gtuxdkisdc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yj20258.top/gtxghwsdir.html

[Q61] 移动平均
来源：http://hz.316326.xyz/gtslkqgjyq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ppjwa.cn/gtggqzgcqb.html

[Q62] 分组占比
来源：http://hz.gogol.net.cn/gtirwrxlvq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yanxiufei.cn/gttbbrlkdg.html

[Q63] 开启事务
来源：http://hz.jinyuanbaomall.cn/gtoypxratc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xingfuxueyuan.xyz/gtwdtepzzn.html

[Q64] 提交事务
来源：http://hz.ybcxt.top/gtbddxsqly.html

COMMIT;
来源：http://hz.52xcode.cn/gtjmrjrici.html

[Q65] 回滚事务
来源：http://hz.zhengqikj.top/gtmsecithl.html

ROLLBACK;
来源：http://hz.52xcode.cn/gtpjbgtywd.html

[Q66] 行锁查询
来源：http://hz.gzhubu.top/gtdhhbqzng.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ybcxt.top/gtgdlwhmrd.html

[Q67] 设置隔离级别
来源：http://hz.xingfuxueyuan.xyz/gtpblmwpwh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.wangdashe.top/gtzxkhholq.html

[Q68] 保存点
来源：http://hz.aibaodan.cn/gtocjhpnks.html

SAVEPOINT sp1;
来源：http://hz.52xcode.cn/gtcpgmpumr.html

ROLLBACK TO sp1;
来源：http://hz.yj20258.top/gtkopxlalb.html

[Q69] 查看执行计划
来源：http://hz.jiagoushi.top/gtybclcoyz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.wangshuangyany.cn/gtwaccdyfc.html

[Q70] 更新统计信息
来源：http://hz.snrcjt.cn/gthdwgwopi.html

ANALYZE TABLE users;
来源：http://hz.yangfankeji.com/gtaseynrew.html

[Q71] 查看建表语句
来源：http://hz.yuxming.cn/gtrljuqwew.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.andypj.xyz/gtlztnmbfk.html

[Q72] 查看索引
来源：http://hz.gogol.net.cn/gtyileqlrw.html

SHOW INDEX FROM users;
来源：http://hz.andypj.xyz/gtgswnjedo.html

[Q73] 查看表状态
来源：http://hz.daria6918.cn/gtuxjltjzx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj20258.top/gtqykepxzu.html

[Q74] 强制使用索引
来源：http://hz.vqdsnc.cn/gtphqzrnus.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.fzhhl.top/gtwxhamlvw.html

[Q75] 日期格式化
来源：http://hz.c1oappe.top/gtxnijhmti.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sysykeji.top/gtzgadhqac.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shzxlz.cn/gtvxaskpuj.html

[Q76] 按天统计
来源：http://hz.hysaishi.cn/gtpshuelse.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sufxvd.cn/gtswovnkph.html

[Q77] 时间加减
来源：http://hz.daxiang520.top/gtiyowzcnw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fzhhl.top/gtptixalmm.html

[Q78] 当前时间
来源：http://hz.zhongyouzk.top/gtrqxnthfn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shuidangran.top/gtaopvubqn.html

[Q79] 字符串拼接
来源：http://hz.ivvv.top/gttinyvwes.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yvedp.cn/gtnzappsbi.html

[Q80] 字符串截取
来源：http://hz.yuxming.cn/gtpynqzxse.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sweek.top/gtreohqjea.html

[Q81] 字符串替换
来源：http://hz.nwbrower.top/gtvebjukbr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.guowangkeji.top/gtqcxogxrk.html

[Q82] 字符长度与字节长度
来源：http://hz.wangdashe.top/gtatjdnqvt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gttgzinxrp.html

[Q83] 大小写转换
来源：http://hz.haohaochexian.top/gtjuzkkcxn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yuanzhike.top/gtmvhrqhsg.html

[Q84] 去除首尾空格
来源：http://hz.vqdsnc.cn/gtmiqufyog.html

SELECT TRIM(name) FROM users;
来源：http://hz.jiagoushi.top/gtmqgbyqjb.html

[Q85] 数值取整
来源：http://hz.sysykeji.top/gtybnzyzxr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.snrcjt.cn/gtovhtomxr.html

[Q86] 读取 JSON 字段
来源：http://hz.daxiang520.top/gtpnnhjpwg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jqgfzy.top/gtvtrecruv.html

[Q87] JSON 字段做条件
来源：http://hz.feifeiyinyue.top/gtrcmsdxvw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ppjwa.cn/gtljfonvnc.html

[Q88] 行转列（条件聚合）
来源：http://hz.ybcxt.top/gtgeqkwznq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cashguo.top/gtgmlfwqbx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hysaishi.cn/gtefzbjuua.html

[Q89] 判断表是否存在
来源：http://hz.jinyuanbaomall.cn/gtlsjtbfyr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hnqzz.top/gtqqdbghhq.html

[Q90] 生成序号列
来源：http://hz.yangfankeji.com/gtcgvvrbwx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.9152youxi.cn/gtosrqobzp.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtlcsbpwlq.html

R. Bash 专题
来源：http://hz.jlsjyb.cn/gtzziscayz.html

================================================================================
来源：http://hz.yangfankeji.com/gtuxizhwfs.html

[R01] shebang 与严格模式
来源：http://hz.nanxinkj.top/gteqohktte.html

#!/usr/bin/env bash
来源：http://hz.zhaomingkeji.xyz/gtilpwqpka.html

set -euo pipefail
来源：http://hz.pycfn.com/gtmpkhdasm.html

[R02] 变量赋值与使用
来源：http://hz.yongpay.top/gtqfopemam.html

name="Tom"; echo "$name"
来源：http://hz.cdnleiting.top/gtqwlnntja.html

[R03] 只读变量
来源：http://hz.zhengqikj.top/gtalmnhzot.html

readonly PI=3.14
来源：http://hz.iojbl.cn/gtvcadzbhl.html

[R04] 位置参数
来源：http://hz.shanyushiyangkeji.top/gtufzcvyux.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.9152youxi.cn/gtxcqtadbw.html

[R05] 参数默认值
来源：http://hz.aizwys.cn/gtobthedml.html

name="${1:-default}"
来源：http://hz.hongshengwenyu.top/gtvmhetyxy.html

[R06] 判断命令是否存在
来源：http://hz.zdqjudy.top/gtqqlgrdyq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sxryk.cn/gtxizrojqk.html

[R07] if 判断文件
来源：http://hz.jlsjyb.cn/gtlcxfjuzs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sufxvd.cn/gtorsxrgbq.html

[R08] 数值比较
来源：http://hz.cdnleiting.top/gtpuvhdjce.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.andypj.xyz/gtvzjkulqp.html

[R09] 字符串比较
来源：http://hz.ydzc1.top/gtawzffjkz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cdnleiting.top/gtcqbzxxwe.html

[R10] 正则匹配
来源：http://hz.ehwqpu.com/gtrahyvroa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.kuanghao11.cn/gtyxachaly.html

[R11] case 多分支
来源：http://hz.kuanghao11.cn/gtsnxkwvxe.html

case "$1" in
来源：http://hz.xuanzx.com/gtnpmvhjro.html

start) echo "启动" ;;
来源：http://hz.jlsjyb.cn/gtnfmnjgge.html

stop)  echo "停止" ;;
来源：http://hz.hongshengwenyu.top/gtkbckcbuy.html

*)     echo "未知命令" ;;
来源：http://hz.smart0.xyz/gtqcjmgetj.html

esac
来源：http://hz.gogol.net.cn/gtphfspjzg.html

[R12] for 遍历文件
来源：http://hz.ybcxt.top/gttlsmdgrk.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenjidiqi.icu/gttbmihqye.html

[R13] for 计数循环
来源：http://hz.fengsongda.top/gtmjxkzyke.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tianlin.xyz/gtlbvdhrkr.html

[R14] C 风格 for
来源：http://hz.hongshengwenyu.top/gtxvrfinne.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.pycfn.com/gthejqxqcr.html

[R15] while 逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtjkscvory.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.kuanghao11.cn/gtkrqlnphh.html

[R16] until 等待条件
来源：http://hz.cheryme.top/gtxycsiwfd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.mhx1999.top/gtwnrmfeps.html

[R17] 数组定义与取值
来源：http://hz.zhijiandao.cn/gtioqtnsvb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cucudq.cn/gtjrcfdspl.html

[R18] 遍历数组
来源：http://hz.zdqjudy.top/gtvthhcrsn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.snrcjt.cn/gtbksewhhh.html

[R19] 数组长度
来源：http://hz.sxryk.cn/gtbiqhmpnr.html

echo "${#arr[@]}"
来源：http://hz.shanyushiyangkeji.top/gtyjbzmbqw.html

[R20] 关联数组（字典）
来源：http://hz.hnqzz.top/gtemtigpts.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.aizwys.cn/gtzmzfkhaf.html

[R21] 字符串长度
来源：http://hz.daxiang520.top/gtqkiwgpsy.html

echo "${#s}"
来源：http://hz.tanke756.top/gtwruwplcu.html

[R22] 截取子串
来源：http://hz.daxiang520.top/gtlbsklkgp.html

echo "${s:0:5}"
来源：http://hz.yuanzhike.top/gtgrvvxpxh.html

[R23] 字符串替换
来源：http://hz.jyoumei.cn/gtijrxrphl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.c1oappe.top/gtcwasjpft.html

[R24] 大小写转换
来源：http://hz.9152youxi.cn/gtqqyaqppx.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cheryme.top/gtujjjrkpr.html

[R25] 去后缀 / 去前缀
来源：http://hz.ydjk.org.cn/gtihbjokmv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yueranfly.top/gtkpioenlb.html

[R26] 命令替换
来源：http://hz.wangshuangyany.cn/gtdgsletip.html

now=$(date +%F); echo "$now"
来源：http://hz.fzhhl.top/gttdfbbcsp.html

[R27] 算术展开
来源：http://hz.zhengqikj.top/gtpdlsvauy.html

echo $((1 + 2 * 3))
来源：http://hz.jyoumei.cn/gtocywcpnn.html

[R28] 浮点运算
来源：http://hz.jinqigfzy.top/gthutjlfzh.html

echo "scale=2; 10/3" | bc
来源：http://hz.daxiang520.top/gtqwwmacsq.html

[R29] 定义函数
来源：http://hz.jianghu66.top/gtskakxcus.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.mhx1999.top/gtrwlnymdy.html

[R30] 函数返回状态码
来源：http://hz.chenzaomai.com/gtwbzulpjh.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhaomingkeji.xyz/gtxgdhosdu.html

[R31] 局部变量
来源：http://hz.sufxvd.cn/gtmqejfgfc.html

f() { local x=1; echo "$x"; }
来源：http://hz.shanyushiyangkeji.top/gtdxbdxmax.html

[R32] 参数个数校验
来源：http://hz.dianchejie.cn/gtewuublts.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hammf.cn/gtzyhokpns.html

[R33] 捕获错误并提示行号
来源：http://hz.chenlongwang.top/gtuhuyvetn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sysykeji.top/gtjlunmlil.html

[R34] 退出时清理
来源：http://hz.hongshengwenyu.top/gtsdzumhzs.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtyiodflsd.html

[R35] 后台执行并等待
来源：http://hz.daria6918.cn/gtvpizpfyj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xuetiantiany.cn/gtqjttyvdc.html

[R36] 并发执行多个任务
来源：http://hz.sysykeji.top/gtjzxbegel.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.dianchejie.cn/gtcqcmqprz.html

[R37] 把输出赋给变量
来源：http://hz.jqgufenzy.top/gtkpejinls.html

files=$(ls -1)
来源：http://hz.sxryk.cn/gtmevrcaof.html

[R38] 管道串联
来源：http://hz.nanxuanxn.top/gtqnxiqzny.html

cat a.txt | grep -i error | wc -l
来源：http://hz.mhx1999.top/gtceoyijbn.html

[R39] 重定向标准输出与错误
来源：http://hz.tian-w.cn/gtpbtewbyw.html

cmd > out.log 2>&1
来源：http://hz.shanyushiyangkeji.top/gtdbhzuamm.html

[R40] 追加写日志
来源：http://hz.hysaishi.cn/gtzdhuuwkm.html

echo "log" >> out.log
来源：http://hz.ydjk.org.cn/gtoagyrnlj.html

[R41] 丢弃输出
来源：http://hz.chenzaomai.com/gtiaaltlkk.html

cmd >/dev/null 2>&1
来源：http://hz.guowangkeji.top/gtdechqfhb.html

[R42] 输入重定向
来源：http://hz.yj202588.top/gttfeecwmd.html

wc -l < a.txt
来源：http://hz.zhongyouzk.top/gthmaeojbk.html

[R43] 按名字查找文件
来源：http://hz.ybcxt.top/gtzswqbtdr.html

find . -name "*.log" -type f
来源：http://hz.yonumen.top/gtazvfhlaz.html

[R44] 按修改时间查找
来源：http://hz.shanyushiyangtech.top/gtbelgkjpd.html

find . -mtime -7 -type f
来源：http://hz.fengsongda.top/gtzvyscann.html

[R45] 批量删除
来源：http://hz.iojbl.cn/gtlyxvulhx.html

find . -name "*.tmp" -delete
来源：http://hz.ivvv.top/gtemsdwnaa.html

[R46] 递归替换文件内容
来源：http://hz.316326.xyz/gtpqhfhjsw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jqgufenzy.top/gtcscwjeoc.html

[R47] sed 单行替换
来源：http://hz.hnqzz.top/gteansovxk.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yonumen.top/gtaikkslwi.html

[R48] awk 取指定列
来源：http://hz.cheryme.top/gtuxzqpitk.html

awk '{print $1, $3}' a.txt
来源：http://hz.jqgufenzy.top/gtwmcfgepk.html

[R49] awk 带条件
来源：http://hz.ivvv.top/gtduhmksfo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.snrcjt.cn/gtmerapcdo.html

[R50] awk 求和
来源：http://hz.xylfe.cn/gtwlpbvnmk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.tian-w.cn/gtppglvqsp.html

[R51] 排序去重取前几
来源：http://hz.jinghuilouyu.cn/gtuxcblivp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cashguo.top/gtgariyybd.html

[R52] 统计行数
来源：http://hz.gzhubu.top/gtzncynleq.html

wc -l a.txt
来源：http://hz.hnqzz.top/gttzfawqgi.html

[R53] 查看文件头与实时尾
来源：http://hz.0kj1m.cn/gtabmofpql.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cheryme.top/gtbdkakpad.html

[R54] 比较两个文件
来源：http://hz.quarkkingdee.top/gtprakfvjh.html

diff a.txt b.txt
来源：http://hz.chenlongwang.top/gtznjxqyor.html

[R55] 压缩与解压
来源：http://hz.yuxming.cn/gtohjoxqbl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.smart0.xyz/gtdkkmsrlr.html

[R56] 远程拷贝
来源：http://hz.xuetiantiany.cn/gtnwpqxcxw.html

scp file user@host:/path/
来源：http://hz.hnxiangtu.top/gtgbpffreg.html

[R57] 远程执行命令
来源：http://hz.xuanzx.com/gtnkpaalei.html

ssh user@host 'uptime'
来源：http://hz.wangshuangyany.cn/gteoxznjji.html

[R58] 下载文件
来源：http://hz.quarkkingdee.top/gtleinqzgk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xziqi.cn/gtdibmfrvx.html

[R59] 发 POST JSON
来源：http://hz.zycfv.cn/gteqwjwhse.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuxming.cn/gtskpwkgzx.html

[R60] 只看 HTTP 状态码
来源：http://hz.svipenyu.cn/gttllvrvvl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.mhx1999.top/gtxlcoetxu.html

[R61] 磁盘占用
来源：http://hz.jinghuilouyu.cn/gtioenmxif.html

df -h;  du -sh *
来源：http://hz.nanxuanxn.top/gtjhqsppfb.html

[R62] 找最占空间的文件
来源：http://hz.cdnleiting.top/gtihwadpfn.html

du -ah . | sort -rh | head -10
来源：http://hz.ywan-chungtsiang.top/gtivnosesu.html

[R63] 内存与进程
来源：http://hz.vqdsnc.cn/gtfjwkrbmp.html

free -h;  ps aux | grep nginx
来源：http://hz.kuanghao11.cn/gtatnbslib.html

[R64] 结束进程
来源：http://hz.zhaomingkeji.xyz/gtcpymabdl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj20258.top/gtixhwioxc.html

[R65] 查看端口占用
来源：http://hz.yvedp.cn/gterctdpds.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.52xcode.cn/gtjwzlhfap.html

[R66] 定时任务
来源：http://hz.wangshuangyany.cn/gtgcacckdd.html

crontab -e;  crontab -l
来源：http://hz.ydzc1.top/gtnicegbgk.html

[R67] 生成随机十六进制串
来源：http://hz.xinyue.icu/gtfztrduuo.html

openssl rand -hex 16
来源：http://hz.zhaomingkeji.xyz/gtmxmbvlxq.html

[R68] 计算文件校验值
来源：http://hz.shanyushiyangtech.top/gtslxqtlba.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.pengpengdd.cyou/gtsqpmmoss.html

[R69] 生成随机密码
来源：http://hz.ydzc1.top/gtduvtcerd.html

head -c 16 /dev/urandom | base64
来源：http://hz.yvedp.cn/gtvparzpvn.html

[R70] 时间戳与互转
来源：http://hz.gotoacloud.top/gtbhdrdgaq.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258888.top/gtbctaehoo.html

[R71] 日期格式化
来源：http://hz.hysaishi.cn/gtnlpuvvgm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenlongwang.top/gthleqvyhu.html

[R72] 等待端口就绪
来源：http://hz.yj20258.top/gtvyigzydx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yuanzhike.top/gtjpgrlhaq.html

[R73] 分割大日志
来源：http://hz.jlsjyb.cn/gtrmwxhyxl.html

split -l 1000 big.log part_
来源：http://hz.shanyushiyangtech.top/gtbqbqrkux.html

[R74] 批量重命名
来源：http://hz.kuanghao11.cn/gtklaolvyd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ivvv.top/gtkdbluxaf.html

[R75] 导出环境变量
来源：http://hz.zhijiandao.cn/gtlkkglkqs.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.smart0.xyz/gticfncugy.html

[R76] 使用临时文件
来源：http://hz.aibaodan.cn/gtrrsjabbr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jyoumei.cn/gtztbnagin.html

[R77] 读取用户输入
来源：http://hz.daxiang520.top/gtjitolzti.html

read -rp "请输入: " ans
来源：http://hz.meibo888.top/gtoigzabyn.html

[R78] 交互式菜单
来源：http://hz.hysaishi.cn/gtvvtiwxth.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinyuanbaomall.cn/gtrprrfngq.html

[R79] 解析命令行选项
来源：http://hz.snrcjt.cn/gtesjcfrjn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhengqikj.top/gtmahwzkcr.html

[R80] 查看脚本执行耗时
来源：http://hz.yueranfly.top/gtnbdzwxbn.html

time ./run.sh
来源：http://hz.zhiwuduotai.top/gtaxwhswtg.html

================================================================================
来源：http://hz.aibaodan.cn/gtnhifddve.html


<!-- 参考信息 -->