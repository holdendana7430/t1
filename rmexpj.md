代发 wailian999

[Q33] 多列分组
来源：http://hz.shanyushiyangtech.top/gttmswozug.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xuanzx.com/gtluhlheza.html

[Q34] 每组取第一条
来源：http://hz.xylfe.cn/gtnsfggppg.html

SELECT * FROM (
来源：http://hz.svipenyu.cn/gteabcrzni.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xingfuxueyuan.xyz/gtyisqvhgk.html

) t WHERE rn = 1;
来源：http://hz.jiagoushi.top/gtxjbsrnpk.html

[Q35] 内连接
来源：http://hz.yanxiufei.cn/gtlhvprfmx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.mhx1999.top/gteimyjnxw.html

[Q36] 左连接
来源：http://hz.zhijiandao.cn/gtdtvvigbe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jianghu66.top/gtswthjtua.html

[Q37] 右连接
来源：http://hz.yj20258.top/gtaetrjhpg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shanyushiyangkeji.top/gtuuhtgvpg.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.guowangkeji.top/gtumzomrwt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shangyingyoupin.top/gtrunwhtro.html

[Q39] 自连接（查上下级）
来源：http://hz.chenlongwang.top/gtnldwuuql.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.wangshuangyany.cn/gtfmgsbpdq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.birdmap.top/gthnrigfry.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.feifeiyinyue.top/gtmtrlvlzz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhiwuduotai.top/gtsylvkejo.html

[Q41] 多表连接
来源：http://hz.feifeiyinyue.top/gtkwwirgkn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xziqi.cn/gtesfndnqo.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinyuanbaomall.cn/gttwaumjsg.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.dianchejie.cn/gttmrghgcl.html

[Q42] 连接条件附加过滤
来源：http://hz.chenlongwang.top/gtcrocqujm.html

SELECT u.name, o.amount FROM users u
来源：http://hz.andypj.xyz/gtgzmubjfr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yvedp.cn/gtfpqmrxor.html

[Q43] 标量子查询
来源：http://hz.yanxiufei.cn/gtknvzoggs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ydzc1.top/gttuzshppn.html

[Q44] IN 子查询
来源：http://hz.tianlin.xyz/gtdgioglpo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.wangshuangyany.cn/gtpcvvadmn.html

[Q45] EXISTS 判断存在
来源：http://hz.52xcode.cn/gttucqfjwg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigfzy.top/gtbcgdponu.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.mhx1999.top/gteeqahora.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.0kj1m.cn/gtdokujfmd.html

[Q47] 与平均值比较
来源：http://hz.iojbl.cn/gtctndqtiz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhiwuduotai.top/gtevuzokrq.html

[Q48] CTE 公用表表达式
来源：http://hz.haohaochexian.top/gtructfsnb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.chenjidiqi.icu/gtlrwoxovg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xingfuxueyuan.xyz/gtdnebwzha.html

[Q49] 更新单行
来源：http://hz.guannengcc.top/gtkmbfwmaq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hfpthk.cn/gtltkxsmxf.html

[Q50] 批量更新
来源：http://hz.zhiwuduotai.top/gtapgfbibr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hongshengwenyu.top/gtthiycjzf.html

[Q51] 用子查询更新
来源：http://hz.gzhubu.top/gtwrgyjfva.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenzaomai.com/gtkpcgoybo.html

[Q52] 删除指定行
来源：http://hz.jinyuanbaomall.cn/gtumlymwdn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ehwqpu.com/gtpswccuas.html

[Q53] 按条件删除
来源：http://hz.pengpengdd.cyou/gtubgymief.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.aizwys.cn/gtignyqcrs.html

[Q54] 清空表
来源：http://hz.yanxiufei.cn/gtpgnvnhvz.html

TRUNCATE TABLE logs;
来源：http://hz.ivvv.top/gtszqavmmi.html

[Q55] 排名（并列占位）
来源：http://hz.jlsjyb.cn/gtdosdnzap.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gogol.net.cn/gtzpfybwxl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.feifeiyinyue.top/gtukthactu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhiwuduotai.top/gteukpmucz.html

[Q57] 行号
来源：http://hz.yongpay.top/gtsufrauqj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.meibo888.top/gtrmtjqbot.html

[Q58] 累计求和
来源：http://hz.sufxvd.cn/gthcdbqngy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sufxvd.cn/gtmaseociu.html

[Q59] 分组内累计
来源：http://hz.cashguo.top/gtnljqvbkb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.birdmap.top/gtocbibuon.html

[Q60] 取上一行 / 下一行
来源：http://hz.chenlongwang.top/gtqlxiwtxo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sysykeji.top/gtrhexptvz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.redwolf501.top/gtvziijnuf.html

[Q61] 移动平均
来源：http://hz.0kj1m.cn/gtslkqorcw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yanxiufei.cn/gtuuxjbkmk.html

[Q62] 分组占比
来源：http://hz.kuanghao11.cn/gtdrqzyeka.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gtxnwicpzx.html

[Q63] 开启事务
来源：http://hz.cqqwz.cn/gtkbuatjfx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.bjfxy.top/gtbusaopvi.html

[Q64] 提交事务
来源：http://hz.daria6918.cn/gteoosivbo.html

COMMIT;
来源：http://hz.daria6918.cn/gtmwccgelu.html

[Q65] 回滚事务
来源：http://hz.daxiang520.top/gtvasjhtvy.html

ROLLBACK;
来源：http://hz.yongpay.top/gtqsxrnhyg.html

[Q66] 行锁查询
来源：http://hz.xingfuxueyuan.xyz/gtyuyqxmsv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.nanxuanxn.top/gtefpztzfm.html

[Q67] 设置隔离级别
来源：http://hz.andypj.xyz/gtghopgkqm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yongpay.top/gtboklusiz.html

[Q68] 保存点
来源：http://hz.cashguo.top/gtvouvizhn.html

SAVEPOINT sp1;
来源：http://hz.bjfxy.top/gtgkkwusrn.html

ROLLBACK TO sp1;
来源：http://hz.316326.xyz/gtdlnlurde.html

[Q69] 查看执行计划
来源：http://hz.snrcjt.cn/gtnbyblwct.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.feifeiyinyue.top/gtoflhhghh.html

[Q70] 更新统计信息
来源：http://hz.aibaodan.cn/gtpxccdqrd.html

ANALYZE TABLE users;
来源：http://hz.sufxvd.cn/gtjjpdryot.html

[Q71] 查看建表语句
来源：http://hz.dianchejie.cn/gtjquuzqku.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.meibo888.top/gtqltacjyx.html

[Q72] 查看索引
来源：http://hz.cashguo.top/gtemysyade.html

SHOW INDEX FROM users;
来源：http://hz.yuxming.cn/gtaqsrsihi.html

[Q73] 查看表状态
来源：http://hz.jlsjyb.cn/gtsptzlfix.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hfpthk.cn/gthpyuzkqr.html

[Q74] 强制使用索引
来源：http://hz.wangshuangyany.cn/gtqzbkckec.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.redwolf501.top/gtvuhzbdpb.html

[Q75] 日期格式化
来源：http://hz.chenjidiqi.icu/gtrxejgjnb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hongshengwenyu.top/gtnypatnhl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jqgfzy.top/gtpsuvtakc.html

[Q76] 按天统计
来源：http://hz.hfpthk.cn/gtmqywjclh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xinyue.icu/gtrztrhsjq.html

[Q77] 时间加减
来源：http://hz.yuxming.cn/gtyhgqajcl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jiagoushi.top/gtzzchgthd.html

[Q78] 当前时间
来源：http://hz.yvedp.cn/gtkdcipflw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xylfe.cn/gtrzbnlvlr.html

[Q79] 字符串拼接
来源：http://hz.yj20258.top/gtmtxkgiym.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.gzhubu.top/gtgonbxdcf.html

[Q80] 字符串截取
来源：http://hz.nanxinkj.top/gtsbjszjvv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xylfe.cn/gtwbingbqt.html

[Q81] 字符串替换
来源：http://hz.cqqwz.cn/gtxiebcdjy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yongpay.top/gttkxxtgtt.html

[Q82] 字符长度与字节长度
来源：http://hz.feifeiyinyue.top/gtzzraqdri.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.wangshuangyany.cn/gthqyzmtrm.html

[Q83] 大小写转换
来源：http://hz.dashuyun.cn/gtitzjbozg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtrhlkoozw.html

[Q84] 去除首尾空格
来源：http://hz.guannengcc.top/gtlcgbpfly.html

SELECT TRIM(name) FROM users;
来源：http://hz.ydjk.org.cn/gtoyiwxcem.html

[Q85] 数值取整
来源：http://hz.pycfn.com/gttuyzsboq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cqqwz.cn/gtwhyvywpp.html

[Q86] 读取 JSON 字段
来源：http://hz.dianchejie.cn/gtwogedmjj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.52xcode.cn/gtyogpvwqz.html

[Q87] JSON 字段做条件
来源：http://hz.redwolf501.top/gtazhzoyay.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hywenlv.cn/gtgixtdrwl.html

[Q88] 行转列（条件聚合）
来源：http://hz.ybcxt.top/gtnzarmacb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jqgfzy.top/gtkntuflvb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinyuanbaomall.cn/gtdygopvof.html

[Q89] 判断表是否存在
来源：http://hz.c1oappe.top/gttekoikkv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.daxiang520.top/gtbogorsel.html

[Q90] 生成序号列
来源：http://hz.andypj.xyz/gtnpwuqzgo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xinyue.icu/gtzzudoxgw.html

================================================================================
来源：http://hz.sweek.top/gtfjdejbgz.html

R. Bash 专题
来源：http://hz.jinyuanbaomall.cn/gtslgyfesv.html

================================================================================
来源：http://hz.wangdashe.top/gtplkhthtr.html

[R01] shebang 与严格模式
来源：http://hz.cashguo.top/gtghvstcxo.html

#!/usr/bin/env bash
来源：http://hz.gaohongyu789.top/gtcewsvjik.html

set -euo pipefail
来源：http://hz.yvedp.cn/gtkfgtmrtm.html

[R02] 变量赋值与使用
来源：http://hz.daria6918.cn/gtwcfocfpo.html

name="Tom"; echo "$name"
来源：http://hz.guannengcc.top/gtnxhmbrbt.html

[R03] 只读变量
来源：http://hz.aizwys.cn/gtfmhupjgp.html

readonly PI=3.14
来源：http://hz.chenlongwang.top/gtsqbnjppn.html

[R04] 位置参数
来源：http://hz.cucudq.cn/gtliefjaon.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cheryme.top/gtvlnfkblc.html

[R05] 参数默认值
来源：http://hz.aibaodan.cn/gtiupglcdf.html

name="${1:-default}"
来源：http://hz.jyoumei.cn/gtlybhlxno.html

[R06] 判断命令是否存在
来源：http://hz.316326.xyz/gtaqbvftjd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hnqzz.top/gtkrzemjcf.html

[R07] if 判断文件
来源：http://hz.nwbrower.top/gttttoaqsg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shangyingyoupin.top/gtcoufqpeh.html

[R08] 数值比较
来源：http://hz.yueranfly.top/gtgaszopub.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.smart0.xyz/gtqhpvwwmz.html

[R09] 字符串比较
来源：http://hz.ybcxt.top/gtaifkiocz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhijiandao.cn/gtflunxejf.html

[R10] 正则匹配
来源：http://hz.haohaochexian.top/gtsqwucwrr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sweek.top/gtkkhbvqko.html

[R11] case 多分支
来源：http://hz.gotoacloud.top/gtzknldsxf.html

case "$1" in
来源：http://hz.hywenlv.cn/gthiyfotib.html

start) echo "启动" ;;
来源：http://hz.ivvv.top/gtyrdwizss.html

stop)  echo "停止" ;;
来源：http://hz.xylfe.cn/gtilkpkija.html

*)     echo "未知命令" ;;
来源：http://hz.wangdashe.top/gtnqdixiyj.html

esac
来源：http://hz.zdqjudy.top/gtncyegopc.html

[R12] for 遍历文件
来源：http://hz.daxiang520.top/gtfrvkkdww.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jyoumei.cn/gtsylphozg.html

[R13] for 计数循环
来源：http://hz.cheryme.top/gtxdpkqtuh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hongshengwenyu.top/gtppqilwdv.html

[R14] C 风格 for
来源：http://hz.ydjk.org.cn/gtevjyitxv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ydzc1.top/gthohkkcxl.html

[R15] while 逐行读文件
来源：http://hz.yj20258.top/gtegpmioze.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.feifeiyinyue.top/gtcnjvdnzr.html

[R16] until 等待条件
来源：http://hz.xylfe.cn/gtgreyaqrc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.chenjidiqi.icu/gtplpeqkvu.html

[R17] 数组定义与取值
来源：http://hz.jyoumei.cn/gtujeotlml.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenlongwang.top/gtraaqyfpy.html

[R18] 遍历数组
来源：http://hz.xylfe.cn/gtwvvgocbr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ehwqpu.com/gtaqvcsxzy.html

[R19] 数组长度
来源：http://hz.yanxiufei.cn/gtbddpnzoi.html

echo "${#arr[@]}"
来源：http://hz.aibaodan.cn/gtijooumtd.html

[R20] 关联数组（字典）
来源：http://hz.zhixingplan.top/gtlcgblvjy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhongyouzk.top/gttktqlwjg.html

[R21] 字符串长度
来源：http://hz.sweek.top/gtwvfptxuq.html

echo "${#s}"
来源：http://hz.pycfn.com/gtbaqizjkq.html

[R22] 截取子串
来源：http://hz.andypj.xyz/gtrzdmhqyu.html

echo "${s:0:5}"
来源：http://hz.xinyue.icu/gtdvuwpjoj.html

[R23] 字符串替换
来源：http://hz.hnxiangtu.top/gtjcgtltnn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.52xcode.cn/gtnfmwpjpr.html

[R24] 大小写转换
来源：http://hz.9152youxi.cn/gtaudirkcj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gotoacloud.top/gttchzusyn.html

[R25] 去后缀 / 去前缀
来源：http://hz.ivvv.top/gtjrcasygg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yuxming.cn/gtokyzzsff.html

[R26] 命令替换
来源：http://hz.hongshengwenyu.top/gtpabakxqv.html

now=$(date +%F); echo "$now"
来源：http://hz.jqgufenzy.top/gtwbjthivi.html

[R27] 算术展开
来源：http://hz.havefunace.top/gtjarjmjai.html

echo $((1 + 2 * 3))
来源：http://hz.zhaomingkeji.xyz/gtbellttuk.html

[R28] 浮点运算
来源：http://hz.c1oappe.top/gtoqgnnszh.html

echo "scale=2; 10/3" | bc
来源：http://hz.316326.xyz/gthgbxhviy.html

[R29] 定义函数
来源：http://hz.jiagoushi.top/gtmxwqbgdu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.aizwys.cn/gthpjpkiif.html

[R30] 函数返回状态码
来源：http://hz.hongshengwenyu.top/gtjfdckoqw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhongyouzk.top/gtbmqbnmdz.html

[R31] 局部变量
来源：http://hz.sweek.top/gtcqoxnpcx.html

f() { local x=1; echo "$x"; }
来源：http://hz.smart0.xyz/gtwysxquog.html

[R32] 参数个数校验
来源：http://hz.hongshengwenyu.top/gthajuyfkf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shzxlz.cn/gtrzovyplx.html

[R33] 捕获错误并提示行号
来源：http://hz.yvedp.cn/gtvefklhns.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhijiandao.cn/gtdqaxqhtd.html

[R34] 退出时清理
来源：http://hz.xinyue.icu/gtbhjnyyiw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.kuanghao11.cn/gtgdzqvpll.html

[R35] 后台执行并等待
来源：http://hz.sufxvd.cn/gtsxofnhom.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ehwqpu.com/gtdvzzlcym.html

[R36] 并发执行多个任务
来源：http://hz.9152youxi.cn/gtciplrcnp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ehwqpu.com/gtksqeosoh.html

[R37] 把输出赋给变量
来源：http://hz.tianlin.xyz/gtbchxxsdn.html

files=$(ls -1)
来源：http://hz.cqqwz.cn/gthqimyonj.html

[R38] 管道串联
来源：http://hz.jinghuilouyu.cn/gthvvcccab.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yuxming.cn/gtygnvwfgo.html

[R39] 重定向标准输出与错误
来源：http://hz.shanyushiyangkeji.top/gtddrkcntl.html

cmd > out.log 2>&1
来源：http://hz.pycfn.com/gtyjwjtbir.html

[R40] 追加写日志
来源：http://hz.zhoulong.xyz/gtldkofiog.html

echo "log" >> out.log
来源：http://hz.andypj.xyz/gtwabfxxwu.html

[R41] 丢弃输出
来源：http://hz.yonumen.top/gtqgptwdvp.html

cmd >/dev/null 2>&1
来源：http://hz.havefunace.top/gtuwfoujqg.html

[R42] 输入重定向
来源：http://hz.pycfn.com/gtapliafhk.html

wc -l < a.txt
来源：http://hz.fzhhl.top/gttrmxhwht.html

[R43] 按名字查找文件
来源：http://hz.c1oappe.top/gtxzeqjjpm.html

find . -name "*.log" -type f
来源：http://hz.zdqjudy.top/gthzydnjsy.html

[R44] 按修改时间查找
来源：http://hz.jianghu66.top/gtkpriwehn.html

find . -mtime -7 -type f
来源：http://hz.tian-w.cn/gtkzegvaax.html

[R45] 批量删除
来源：http://hz.yuanzhike.top/gtwgrbciyr.html

find . -name "*.tmp" -delete
来源：http://hz.guannengcc.top/gtrezlgprv.html

[R46] 递归替换文件内容
来源：http://hz.ydjk.org.cn/gtaoosqoqh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.svipenyu.cn/gtlnustqop.html

[R47] sed 单行替换
来源：http://hz.havefunace.top/gtmzpkecor.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.andypj.xyz/gteytxhdgt.html

[R48] awk 取指定列
来源：http://hz.yongpay.top/gtattqleey.html

awk '{print $1, $3}' a.txt
来源：http://hz.zycfv.cn/gtuwhntywd.html

[R49] awk 带条件
来源：http://hz.ybcxt.top/gtvzevebib.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cqqwz.cn/gteyvzadek.html

[R50] awk 求和
来源：http://hz.wangdashe.top/gtshbxzmka.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cashguo.top/gtsriotxjy.html

[R51] 排序去重取前几
来源：http://hz.xziqi.cn/gtffxhukqb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj20258888.top/gtabyisadw.html

[R52] 统计行数
来源：http://hz.fzhhl.top/gtvhgwddgt.html

wc -l a.txt
来源：http://hz.ybcxt.top/gtwfnwwmiw.html

[R53] 查看文件头与实时尾
来源：http://hz.iojbl.cn/gtrkfjnoxx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jiagoushi.top/gtreorlitj.html

[R54] 比较两个文件
来源：http://hz.jinqigfzy.top/gthvwayynv.html

diff a.txt b.txt
来源：http://hz.hfpthk.cn/gtdrtgmgue.html

[R55] 压缩与解压
来源：http://hz.hfpthk.cn/gtlldcjoyy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yuxming.cn/gtjnrcibvu.html

[R56] 远程拷贝
来源：http://hz.ppjwa.cn/gtsogrwlju.html

scp file user@host:/path/
来源：http://hz.hnxiangtu.top/gtjnhltxmb.html

[R57] 远程执行命令
来源：http://hz.tanke756.top/gtbcnavlrn.html

ssh user@host 'uptime'
来源：http://hz.daria6918.cn/gtnuzcrjii.html

[R58] 下载文件
来源：http://hz.xuetiantiany.cn/gtlqqcnsyf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.haohaochexian.top/gtqtrgdgbp.html

[R59] 发 POST JSON
来源：http://hz.gaohongyu789.top/gtvhrbzqld.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.aibaodan.cn/gtcksghdeh.html

[R60] 只看 HTTP 状态码
来源：http://hz.yueranfly.top/gtzxifhgae.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yvedp.cn/gtedahobxl.html

[R61] 磁盘占用
来源：http://hz.yanxiufei.cn/gtnixtufub.html

df -h;  du -sh *
来源：http://hz.andypj.xyz/gtavalfcqx.html

[R62] 找最占空间的文件
来源：http://hz.birdmap.top/gtbhvhisxt.html

du -ah . | sort -rh | head -10
来源：http://hz.dashuyun.cn/gtvxeyldki.html

[R63] 内存与进程
来源：http://hz.chenlongwang.top/gtsphylpll.html

free -h;  ps aux | grep nginx
来源：http://hz.cqqwz.cn/gthxdvoywi.html

[R64] 结束进程
来源：http://hz.cqqwz.cn/gtiuhtmnmr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cashguo.top/gterrunrzy.html

[R65] 查看端口占用
来源：http://hz.cashguo.top/gtfftyodxk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sufxvd.cn/gtxvbksbcf.html

[R66] 定时任务
来源：http://hz.yvedp.cn/gtzcbymerw.html

crontab -e;  crontab -l
来源：http://hz.zhaomingkeji.xyz/gtbtvvpsao.html

[R67] 生成随机十六进制串
来源：http://hz.jiagoushi.top/gtknzcnukw.html

openssl rand -hex 16
来源：http://hz.ivvv.top/gtlqeeksvr.html

[R68] 计算文件校验值
来源：http://hz.xuanzx.com/gtviogkqva.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hywenlv.cn/gtejmfwooc.html

[R69] 生成随机密码
来源：http://hz.jiagoushi.top/gtsbmurpdo.html

head -c 16 /dev/urandom | base64
来源：http://hz.gotoacloud.top/gthrkuymrr.html

[R70] 时间戳与互转
来源：http://hz.yuxming.cn/gtcltlxwzj.html

date +%s;  date -d @1700000000
来源：http://hz.hnxiangtu.top/gtgkrhjmhy.html

[R71] 日期格式化
来源：http://hz.jianghu66.top/gtpmeahmiy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.snrcjt.cn/gtmuktzsac.html

[R72] 等待端口就绪
来源：http://hz.xuetiantiany.cn/gtscdmmkvr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ybcxt.top/gtkuwnfdvc.html

[R73] 分割大日志
来源：http://hz.jianghu66.top/gtafmnvnzv.html

split -l 1000 big.log part_
来源：http://hz.fzhhl.top/gtfompqwaj.html

[R74] 批量重命名
来源：http://hz.shanyushiyangtech.top/gtztzpiqrq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.quarkkingdee.top/gtllxjvizw.html

[R75] 导出环境变量
来源：http://hz.snrcjt.cn/gtorandkou.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sysykeji.top/gtkdepwnfn.html

[R76] 使用临时文件
来源：http://hz.shanyushiyangtech.top/gthrctlumy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.aizwys.cn/gtdhrtydui.html

[R77] 读取用户输入
来源：http://hz.nwbrower.top/gtypwjxfgd.html

read -rp "请输入: " ans
来源：http://hz.guowangkeji.top/gthdunuxhl.html

[R78] 交互式菜单
来源：http://hz.nanxinkj.top/gtvdhmzkcd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sxryk.cn/gtdvnrpimr.html

[R79] 解析命令行选项
来源：http://hz.smart0.xyz/gtqcbbjghq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.316326.xyz/gtuvdwffjb.html

[R80] 查看脚本执行耗时
来源：http://hz.wangdashe.top/gtxxvloeis.html

time ./run.sh
来源：http://hz.hammf.cn/gtceglzfht.html

================================================================================
来源：http://hz.zhixingplan.top/gtndnusctw.html

S. C / C++ 专题
来源：http://hz.guowangkeji.top/gtophiuyjv.html

================================================================================
来源：http://hz.birdmap.top/gtndtoqoey.html

[S01] C：Hello World
来源：http://hz.haohaochexian.top/gtnygiapmi.html

#include <stdio.h>
来源：http://hz.shzxlz.cn/gttadsuxim.html


<!-- 参考信息 -->