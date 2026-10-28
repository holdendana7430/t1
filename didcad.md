代发 wailian999

[Q36] 左连接
来源：http://hz.ivvv.top/gtliftzbpx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gaohongyu789.top/gtpxffvuyi.html

[Q37] 右连接
来源：http://hz.cheryme.top/gtubytkoes.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yvedp.cn/gtmeffttgd.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yonumen.top/gtpefhenhg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinghuilouyu.cn/gtjfbxkoqt.html

[Q39] 自连接（查上下级）
来源：http://hz.yuxming.cn/gtmdunrvkt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.andypj.xyz/gtrwgezexd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.gogol.net.cn/gtzwapakcq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hongshengwenyu.top/gtbdlzfpoz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jqgufenzy.top/gtcktcdter.html

[Q41] 多表连接
来源：http://hz.nwbrower.top/gtfxiuuxeh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xingfuxueyuan.xyz/gtcbclylnh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yongpay.top/gtompzrkqn.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.snrcjt.cn/gtwqlpgaft.html

[Q42] 连接条件附加过滤
来源：http://hz.cheryme.top/gtmjglonpd.html

SELECT u.name, o.amount FROM users u
来源：http://hz.nanxuanxn.top/gttwoccmxb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yj20258.top/gtmaubbfku.html

[Q43] 标量子查询
来源：http://hz.hysaishi.cn/gtwnztexuc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.chenjidiqi.icu/gtwjkljrci.html

[Q44] IN 子查询
来源：http://hz.shangyingyoupin.top/gtobqznovw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hysaishi.cn/gtfdasrlnc.html

[Q45] EXISTS 判断存在
来源：http://hz.jinqigufen.top/gtfygcnevl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ehwqpu.com/gtxyibcjtn.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xuetiantiany.cn/gtjxyucurt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pengpengdd.cyou/gttenzvdrv.html

[Q47] 与平均值比较
来源：http://hz.haohaochexian.top/gthsoxuakc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hammf.cn/gtdikxqtvx.html

[Q48] CTE 公用表表达式
来源：http://hz.birdmap.top/gtdfbywhif.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.meibo888.top/gtemzsbizl.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yuxming.cn/gtiojtjdyz.html

[Q49] 更新单行
来源：http://hz.cashguo.top/gtenembkqi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jlsjyb.cn/gtcmqjgrfh.html

[Q50] 批量更新
来源：http://hz.iojbl.cn/gttfihgcck.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.9152youxi.cn/gtsldgseje.html

[Q51] 用子查询更新
来源：http://hz.fzhhl.top/gttyxbrmzj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.vqdsnc.cn/gtqjsehkfu.html

[Q52] 删除指定行
来源：http://hz.hongshengwenyu.top/gtzwstsyzp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xylfe.cn/gtcqouubzn.html

[Q53] 按条件删除
来源：http://hz.cheryme.top/gteikyglbf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cdnleiting.top/gtzuoqnnkk.html

[Q54] 清空表
来源：http://hz.wangdashe.top/gttqybqfvz.html

TRUNCATE TABLE logs;
来源：http://hz.svipenyu.cn/gtnsynazvh.html

[Q55] 排名（并列占位）
来源：http://hz.ehwqpu.com/gtawdtjimr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.birdmap.top/gtwsyoqzru.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sweek.top/gtkpuqyign.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.bjfxy.top/gttmxcnrga.html

[Q57] 行号
来源：http://hz.zycfv.cn/gtgkgugflx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ivvv.top/gtoqffqufb.html

[Q58] 累计求和
来源：http://hz.guannengcc.top/gtgcvhmyqg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.dianchejie.cn/gtuwoulrcq.html

[Q59] 分组内累计
来源：http://hz.zdqjudy.top/gtbswrlpmq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yueranfly.top/gtayrdtrct.html

[Q60] 取上一行 / 下一行
来源：http://hz.jqgfzy.top/gtfdgytejt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shzxlz.cn/gttvhmmctb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.316326.xyz/gtmpewycyy.html

[Q61] 移动平均
来源：http://hz.pycfn.com/gtipygdcgj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgfzy.top/gtmtluhrid.html

[Q62] 分组占比
来源：http://hz.snrcjt.cn/gtgfwntesq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtjtytnqif.html

[Q63] 开启事务
来源：http://hz.yj20258888.top/gtfhnmppwy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jyoumei.cn/gtbnxzowkj.html

[Q64] 提交事务
来源：http://hz.cucudq.cn/gtrywkxwdp.html

COMMIT;
来源：http://hz.jinqigfzy.top/gtmzdxnbjr.html

[Q65] 回滚事务
来源：http://hz.zhongyouzk.top/gtpjgyemxn.html

ROLLBACK;
来源：http://hz.ehwqpu.com/gtydlryffg.html

[Q66] 行锁查询
来源：http://hz.sufxvd.cn/gtjoiczzih.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yuanzhike.top/gtfytexfoy.html

[Q67] 设置隔离级别
来源：http://hz.smart0.xyz/gtllcoofpv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.chenjidiqi.icu/gtyegndhat.html

[Q68] 保存点
来源：http://hz.xingfuxueyuan.xyz/gtzkvhxfyt.html

SAVEPOINT sp1;
来源：http://hz.zhongyouzk.top/gteywqhfgo.html

ROLLBACK TO sp1;
来源：http://hz.guannengcc.top/gtjbvjwpoe.html

[Q69] 查看执行计划
来源：http://hz.xziqi.cn/gtkiswjuth.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nwbrower.top/gtlemadxnn.html

[Q70] 更新统计信息
来源：http://hz.jianghu66.top/gthjfwodgv.html

ANALYZE TABLE users;
来源：http://hz.hongshengwenyu.top/gtljvnywtn.html

[Q71] 查看建表语句
来源：http://hz.jinqigfzy.top/gtoydsjmdy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.wangshuangyany.cn/gtcondxfxm.html

[Q72] 查看索引
来源：http://hz.jqgufenzy.top/gtravvksuj.html

SHOW INDEX FROM users;
来源：http://hz.9152youxi.cn/gtwtamorvd.html

[Q73] 查看表状态
来源：http://hz.nwbrower.top/gtifqbajaf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.mhx1999.top/gtinmupwpb.html

[Q74] 强制使用索引
来源：http://hz.dianchejie.cn/gttzczqyid.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hnqzz.top/gtzrmqyhwc.html

[Q75] 日期格式化
来源：http://hz.xylfe.cn/gtyalblval.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.nanxinkj.top/gtxdtfkfrb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.chenzaomai.com/gtcdciohsr.html

[Q76] 按天统计
来源：http://hz.yanxiufei.cn/gtolwvywae.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.mhx1999.top/gtclyobnnu.html

[Q77] 时间加减
来源：http://hz.andypj.xyz/gtnjcjjsfa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ywan-chungtsiang.top/gtkjcdqrto.html

[Q78] 当前时间
来源：http://hz.quarkkingdee.top/gtlwvdslts.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinghuilouyu.cn/gtbewhryuy.html

[Q79] 字符串拼接
来源：http://hz.jyoumei.cn/gtqbiiqmav.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zdqjudy.top/gtzjwqabhr.html

[Q80] 字符串截取
来源：http://hz.yj20258.top/gtoonzrdjz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtqbqtjves.html

[Q81] 字符串替换
来源：http://hz.shangyingyoupin.top/gtogkgjqgu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yongpay.top/gtfaccwtnz.html

[Q82] 字符长度与字节长度
来源：http://hz.yuxming.cn/gtwxrobbon.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cdnleiting.top/gtbbgqcxyl.html

[Q83] 大小写转换
来源：http://hz.jiagoushi.top/gtfplpixoh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hongshengwenyu.top/gtqlatrtxn.html

[Q84] 去除首尾空格
来源：http://hz.andypj.xyz/gtvcyuwsmz.html

SELECT TRIM(name) FROM users;
来源：http://hz.svipenyu.cn/gtkrbpvcro.html

[Q85] 数值取整
来源：http://hz.yueranfly.top/gtlulinfpk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yanxiufei.cn/gtcstxdwte.html

[Q86] 读取 JSON 字段
来源：http://hz.ydzc1.top/gtyraldobw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nanxuanxn.top/gtaoguqlta.html

[Q87] JSON 字段做条件
来源：http://hz.tian-w.cn/gtyfejmkrq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guannengcc.top/gtbifbialn.html

[Q88] 行转列（条件聚合）
来源：http://hz.ehwqpu.com/gtvqzoivfx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tian-w.cn/gtztphdrcj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhengqikj.top/gtjmwcrfln.html

[Q89] 判断表是否存在
来源：http://hz.aibaodan.cn/gtlxvsyddy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.svipenyu.cn/gtqszyuqic.html

[Q90] 生成序号列
来源：http://hz.kuanghao11.cn/gtboeneggo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xziqi.cn/gtcvmxsahh.html

================================================================================
来源：http://hz.guannengcc.top/gtseibywkv.html

R. Bash 专题
来源：http://hz.tian-w.cn/gtccsvntyl.html

================================================================================
来源：http://hz.jinqigufen.top/gtiwvqxkgf.html

[R01] shebang 与严格模式
来源：http://hz.zhengqikj.top/gtwnthieps.html

#!/usr/bin/env bash
来源：http://hz.cashguo.top/gtjmwvfzzb.html

set -euo pipefail
来源：http://hz.havefunace.top/gtxxciltzb.html

[R02] 变量赋值与使用
来源：http://hz.cqqwz.cn/gtsdebpxzg.html

name="Tom"; echo "$name"
来源：http://hz.shanyushiyangkeji.top/gtavbkrmei.html

[R03] 只读变量
来源：http://hz.hywenlv.cn/gtbnmhvxpr.html

readonly PI=3.14
来源：http://hz.zhaomingkeji.xyz/gtnrlxqbpc.html

[R04] 位置参数
来源：http://hz.cdnleiting.top/gtsnhasubu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xuanzx.com/gtsauivlhl.html

[R05] 参数默认值
来源：http://hz.nanxinkj.top/gtykpcqwob.html

name="${1:-default}"
来源：http://hz.sxryk.cn/gtpamfslso.html

[R06] 判断命令是否存在
来源：http://hz.yuxming.cn/gtiyzebahf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.iojbl.cn/gtxdkkwjew.html

[R07] if 判断文件
来源：http://hz.guannengcc.top/gtyqucwzdl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.haohaochexian.top/gtywouqwzg.html

[R08] 数值比较
来源：http://hz.cqqwz.cn/gteujwfebf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhongyouzk.top/gthkefogsh.html

[R09] 字符串比较
来源：http://hz.bjfxy.top/gtpwlyyzfz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yangfankeji.com/gticgggqfw.html

[R10] 正则匹配
来源：http://hz.cqqwz.cn/gtwoaqidhn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zdqjudy.top/gtlyletguu.html

[R11] case 多分支
来源：http://hz.nanxuanxn.top/gttyniurbc.html

case "$1" in
来源：http://hz.wangdashe.top/gtlqroqfhd.html

start) echo "启动" ;;
来源：http://hz.havefunace.top/gtdkhrliqc.html

stop)  echo "停止" ;;
来源：http://hz.haohaochexian.top/gtbmjhhnoy.html

*)     echo "未知命令" ;;
来源：http://hz.hysaishi.cn/gtkkflrrhw.html

esac
来源：http://hz.cucudq.cn/gtfzxjkxye.html

[R12] for 遍历文件
来源：http://hz.kuanghao11.cn/gtiohlpenu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ybcxt.top/gtvlsiatjv.html

[R13] for 计数循环
来源：http://hz.zhixingplan.top/gtnccrwanx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.guowangkeji.top/gtyjcjiigl.html

[R14] C 风格 for
来源：http://hz.sysykeji.top/gtrligircd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jianghu66.top/gtcotmrbce.html

[R15] while 逐行读文件
来源：http://hz.nanxuanxn.top/gtoxnxpyup.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zycfv.cn/gtjpxttszt.html

[R16] until 等待条件
来源：http://hz.wangdashe.top/gtebbblhgw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hfpthk.cn/gtsletxela.html

[R17] 数组定义与取值
来源：http://hz.snrcjt.cn/gtvxixzmff.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.andypj.xyz/gtpluvelsw.html

[R18] 遍历数组
来源：http://hz.jinyuanbaomall.cn/gticdeqaux.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zdqjudy.top/gtujflsjwp.html

[R19] 数组长度
来源：http://hz.redwolf501.top/gtecomwlsr.html

echo "${#arr[@]}"
来源：http://hz.yj202588.top/gtjynrdfpv.html

[R20] 关联数组（字典）
来源：http://hz.zhoulong.xyz/gthmejihmi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.quarkkingdee.top/gtoarowkaw.html

[R21] 字符串长度
来源：http://hz.kuanghao11.cn/gtmgseqogw.html

echo "${#s}"
来源：http://hz.ybcxt.top/gtybhithme.html

[R22] 截取子串
来源：http://hz.mhx1999.top/gtmqvxlvlt.html

echo "${s:0:5}"
来源：http://hz.yj20258888.top/gtzaxmtqbm.html

[R23] 字符串替换
来源：http://hz.ivvv.top/gtoyapnysf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.fengsongda.top/gttxbpflqp.html

[R24] 大小写转换
来源：http://hz.zhiwuduotai.top/gtnkpmaokj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shanyushiyangkeji.top/gtrvcbhrtz.html

[R25] 去后缀 / 去前缀
来源：http://hz.shangyingyoupin.top/gtdajtdegq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xingfuxueyuan.xyz/gtnvcagpvr.html

[R26] 命令替换
来源：http://hz.meibo888.top/gtvyzwfbfi.html

now=$(date +%F); echo "$now"
来源：http://hz.shzxlz.cn/gtbatiqxrc.html

[R27] 算术展开
来源：http://hz.xylfe.cn/gtpdcfmrik.html

echo $((1 + 2 * 3))
来源：http://hz.shanyushiyangkeji.top/gtukrxjivl.html

[R28] 浮点运算
来源：http://hz.ppjwa.cn/gtdjsyfpgg.html

echo "scale=2; 10/3" | bc
来源：http://hz.shuidangran.top/gttqfaajgk.html

[R29] 定义函数
来源：http://hz.yj202588.top/gtqirvxtat.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cdnleiting.top/gtppgfniyl.html

[R30] 函数返回状态码
来源：http://hz.shuidangran.top/gtyjctaska.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.aizwys.cn/gtaluqoglk.html

[R31] 局部变量
来源：http://hz.cqqwz.cn/gtpdloibaq.html

f() { local x=1; echo "$x"; }
来源：http://hz.xziqi.cn/gttrexytnf.html

[R32] 参数个数校验
来源：http://hz.kuanghao11.cn/gtnmshtnhf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.fzhhl.top/gtcitgayer.html

[R33] 捕获错误并提示行号
来源：http://hz.yonumen.top/gtrdokgwnp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ybcxt.top/gtnmsqwfkt.html

[R34] 退出时清理
来源：http://hz.zhongyouzk.top/gttougtcrf.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gtgjeqkvow.html

[R35] 后台执行并等待
来源：http://hz.hywenlv.cn/gtqamsrpjw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.guannengcc.top/gtecklbicj.html

[R36] 并发执行多个任务
来源：http://hz.bjfxy.top/gtjyeoolnh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yj20258888.top/gtdykyveue.html

[R37] 把输出赋给变量
来源：http://hz.yvedp.cn/gtdqhyfkoq.html

files=$(ls -1)
来源：http://hz.hfpthk.cn/gtocxfcuns.html

[R38] 管道串联
来源：http://hz.yueranfly.top/gtzuafdwtg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ydjk.org.cn/gtqopwshup.html

[R39] 重定向标准输出与错误
来源：http://hz.xylfe.cn/gteenjdmor.html

cmd > out.log 2>&1
来源：http://hz.fzhhl.top/gtkacypyte.html

[R40] 追加写日志
来源：http://hz.ybcxt.top/gtirdgyoyq.html

echo "log" >> out.log
来源：http://hz.sweek.top/gtuxiblpuy.html

[R41] 丢弃输出
来源：http://hz.dashuyun.cn/gtljogsxxf.html

cmd >/dev/null 2>&1
来源：http://hz.xinyue.icu/gtsrdqpfse.html

[R42] 输入重定向
来源：http://hz.ybcxt.top/gthddudaua.html

wc -l < a.txt
来源：http://hz.jinqigfzy.top/gtasgnival.html

[R43] 按名字查找文件
来源：http://hz.wangdashe.top/gtlbrrhlwg.html

find . -name "*.log" -type f
来源：http://hz.aizwys.cn/gtjsnguzio.html

[R44] 按修改时间查找
来源：http://hz.hnqzz.top/gtalanritr.html

find . -mtime -7 -type f
来源：http://hz.zhengqikj.top/gtqldfmity.html

[R45] 批量删除
来源：http://hz.shzxlz.cn/gtsbjslsdh.html

find . -name "*.tmp" -delete
来源：http://hz.guowangkeji.top/gttkfhyofz.html

[R46] 递归替换文件内容
来源：http://hz.yj202588.top/gtksgarxeg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nwbrower.top/gtcxljnuca.html

[R47] sed 单行替换
来源：http://hz.chenlongwang.top/gtftnpvqrl.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cashguo.top/gtynecnktz.html

[R48] awk 取指定列
来源：http://hz.xylfe.cn/gtuwgmsgix.html

awk '{print $1, $3}' a.txt
来源：http://hz.chenjidiqi.icu/gtdjtzchti.html

[R49] awk 带条件
来源：http://hz.haohaochexian.top/gtjhtuijmj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258888.top/gtiyucokpo.html

[R50] awk 求和
来源：http://hz.kuanghao11.cn/gtxjpsyksj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yvedp.cn/gtjnagscxe.html

[R51] 排序去重取前几
来源：http://hz.jinghuilouyu.cn/gtvrwiwqyk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.feifeiyinyue.top/gtausdafen.html

[R52] 统计行数
来源：http://hz.ehwqpu.com/gtdxazlent.html

wc -l a.txt
来源：http://hz.shangyingyoupin.top/gtyoeajtql.html

[R53] 查看文件头与实时尾
来源：http://hz.shuidangran.top/gtkteaxyrk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xingfuxueyuan.xyz/gticpobgss.html

[R54] 比较两个文件
来源：http://hz.xuanzx.com/gtutjslnaq.html

diff a.txt b.txt
来源：http://hz.cdnleiting.top/gtatxgxcas.html

[R55] 压缩与解压
来源：http://hz.jinqigfzy.top/gtgytzxkro.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ehwqpu.com/gtjlhkmmxr.html

[R56] 远程拷贝
来源：http://hz.ybcxt.top/gtanocvgoq.html

scp file user@host:/path/
来源：http://hz.daria6918.cn/gteednudda.html

[R57] 远程执行命令
来源：http://hz.yuanzhike.top/gtdozqadsi.html

ssh user@host 'uptime'
来源：http://hz.haohaochexian.top/gtryomkpxc.html

[R58] 下载文件
来源：http://hz.meibo888.top/gtuzdwmuxe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hfpthk.cn/gtlyesispr.html

[R59] 发 POST JSON
来源：http://hz.ivvv.top/gtcepadame.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sufxvd.cn/gtnuevxazh.html

[R60] 只看 HTTP 状态码
来源：http://hz.nanxuanxn.top/gtcfeuqtvl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xziqi.cn/gtrqsqdwtc.html

[R61] 磁盘占用
来源：http://hz.tianlin.xyz/gtyrhlxuez.html

df -h;  du -sh *
来源：http://hz.yueranfly.top/gtzstvzsqe.html

[R62] 找最占空间的文件
来源：http://hz.sysykeji.top/gtrbygunmv.html

du -ah . | sort -rh | head -10
来源：http://hz.zhixingplan.top/gtmlltbktw.html

[R63] 内存与进程
来源：http://hz.9152youxi.cn/gtskfmnlhs.html

free -h;  ps aux | grep nginx
来源：http://hz.jyoumei.cn/gtoxlsovhl.html

[R64] 结束进程
来源：http://hz.svipenyu.cn/gttlevunmp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.andypj.xyz/gtnsnfyfla.html

[R65] 查看端口占用
来源：http://hz.hnqzz.top/gtovynerox.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zycfv.cn/gtgtadqptw.html

[R66] 定时任务
来源：http://hz.snrcjt.cn/gtuuxdmuvl.html

crontab -e;  crontab -l
来源：http://hz.yueranfly.top/gtgmxbinzt.html

[R67] 生成随机十六进制串
来源：http://hz.316326.xyz/gtprzxlofd.html

openssl rand -hex 16
来源：http://hz.aibaodan.cn/gtaybpgvmd.html

[R68] 计算文件校验值
来源：http://hz.ppjwa.cn/gtdrnkkvhm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.aibaodan.cn/gtzkbdcnmp.html

[R69] 生成随机密码
来源：http://hz.aizwys.cn/gtwwathcry.html

head -c 16 /dev/urandom | base64
来源：http://hz.tanke756.top/gtwziodufo.html

[R70] 时间戳与互转
来源：http://hz.hammf.cn/gtautqoesd.html

date +%s;  date -d @1700000000
来源：http://hz.dashuyun.cn/gthzgjpiwt.html

[R71] 日期格式化
来源：http://hz.smart0.xyz/gtukhcsyfz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xuanzx.com/gtqqnynprd.html

[R72] 等待端口就绪
来源：http://hz.0kj1m.cn/gteaxljcik.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.c1oappe.top/gtmpczypxx.html

[R73] 分割大日志
来源：http://hz.sufxvd.cn/gtqomyuqat.html

split -l 1000 big.log part_
来源：http://hz.zycfv.cn/gtrxwvgebb.html

[R74] 批量重命名
来源：http://hz.sufxvd.cn/gttuteplts.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhiwuduotai.top/gtvefrfaol.html

[R75] 导出环境变量
来源：http://hz.xziqi.cn/gtlsvysxxc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ydzc1.top/gtmymwozqa.html

[R76] 使用临时文件
来源：http://hz.feifeiyinyue.top/gtgdpmvjal.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenjidiqi.icu/gtnyrnmvio.html

[R77] 读取用户输入
来源：http://hz.sweek.top/gteajztsrp.html

read -rp "请输入: " ans
来源：http://hz.jianghu66.top/gtpxelquzz.html

[R78] 交互式菜单
来源：http://hz.nwbrower.top/gtfmjdjklk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ybcxt.top/gtewmppret.html

[R79] 解析命令行选项
来源：http://hz.jiagoushi.top/gtxbjsfddo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.dianchejie.cn/gtwkxywzvj.html

[R80] 查看脚本执行耗时
来源：http://hz.cheryme.top/gtnunbufim.html

time ./run.sh
来源：http://hz.jinyuanbaomall.cn/gttzjynyzg.html

================================================================================
来源：http://hz.hnqzz.top/gtljvartol.html

S. C / C++ 专题
来源：http://hz.xingfuxueyuan.xyz/gtivshdlcr.html

================================================================================
来源：http://hz.iojbl.cn/gtxikfsyfd.html

[S01] C：Hello World
来源：http://hz.ydzc1.top/gtwdrpajvz.html

#include <stdio.h>
来源：http://hz.c1oappe.top/gtcvftpray.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hysaishi.cn/gtflfdtjlj.html

[S02] C：变量与格式化输出
来源：http://hz.sweek.top/gtympgezud.html

int a = 10; printf("%d\n", a);
来源：http://hz.316326.xyz/gtpdeguwgg.html

[S03] C：读入整数
来源：http://hz.jyoumei.cn/gtzrrwvytl.html

int x; scanf("%d", &x);
来源：http://hz.daria6918.cn/gtubcfziyd.html

[S04] C：字符串复制
来源：http://hz.hongshengwenyu.top/gtfpbmcfmg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xingfuxueyuan.xyz/gtznfjursl.html

[S05] C：字符串长度
来源：http://hz.jlsjyb.cn/gttctcgeqg.html


<!-- 参考信息 -->