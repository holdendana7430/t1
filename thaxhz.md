代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhengqikj.top/gtjbqytefr.html

[Q32] 分组拼接字符串
来源：http://hz.quarkkingdee.top/gtdrpkdoqy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.chenzaomai.com/gtzyvebyqj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.wangshuangyany.cn/gththsbkbk.html

[Q33] 多列分组
来源：http://hz.xingfuxueyuan.xyz/gtztddbnou.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xinyue.icu/gthwsvndpc.html

[Q34] 每组取第一条
来源：http://hz.ppjwa.cn/gtbomqgxzs.html

SELECT * FROM (
来源：http://hz.yonumen.top/gttygqsyyg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinqigfzy.top/gtbjifmdvn.html

) t WHERE rn = 1;
来源：http://hz.mhx1999.top/gtousdccuy.html

[Q35] 内连接
来源：http://hz.ybcxt.top/gtupxqftrb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jianghu66.top/gtlextcxqw.html

[Q36] 左连接
来源：http://hz.cucudq.cn/gtogoyqkbd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nwbrower.top/gtaibdukwu.html

[Q37] 右连接
来源：http://hz.gogol.net.cn/gtaykaqagx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.iojbl.cn/gtadyijwzk.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gaohongyu789.top/gtollppydm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jiagoushi.top/gtgbsronge.html

[Q39] 自连接（查上下级）
来源：http://hz.haohaochexian.top/gtykkpntsm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xinyue.icu/gthijxxgwe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ydjk.org.cn/gtnnmsiern.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinyuanbaomall.cn/gtzixzvphq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jqgufenzy.top/gtihatsdoz.html

[Q41] 多表连接
来源：http://hz.yueranfly.top/gtfsmoyfwa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.quarkkingdee.top/gtbigpjfhb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cheryme.top/gtsfldhkpd.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yj202588.top/gtcvpyychs.html

[Q42] 连接条件附加过滤
来源：http://hz.ppjwa.cn/gtsmczqzwo.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shuidangran.top/gtexkeofjw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ivvv.top/gtecywlbtb.html

[Q43] 标量子查询
来源：http://hz.cashguo.top/gtsjsgnwhn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhixingplan.top/gtnxyomugo.html

[Q44] IN 子查询
来源：http://hz.ivvv.top/gtkxcgamin.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jiagoushi.top/gthhcdctak.html

[Q45] EXISTS 判断存在
来源：http://hz.bjfxy.top/gtogrfvxda.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gogol.net.cn/gtdhmknelz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.haohaochexian.top/gtvpzhgsgs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gaohongyu789.top/gtsxblwoxp.html

[Q47] 与平均值比较
来源：http://hz.shangyingyoupin.top/gtmhxdurpa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jqgfzy.top/gtozorgsej.html

[Q48] CTE 公用表表达式
来源：http://hz.yj20258888.top/gtnwfmerzi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xuanzx.com/gtdooihzyu.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.guowangkeji.top/gtveemthyk.html

[Q49] 更新单行
来源：http://hz.tanke756.top/gtojdnrpql.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yueranfly.top/gtenszyvne.html

[Q50] 批量更新
来源：http://hz.smart0.xyz/gtiocnjdsn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.snrcjt.cn/gtebitowyc.html

[Q51] 用子查询更新
来源：http://hz.wangshuangyany.cn/gtlpctqmpz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.svipenyu.cn/gtpcxlscmg.html

[Q52] 删除指定行
来源：http://hz.xuetiantiany.cn/gtowlslvvm.html

DELETE FROM users WHERE id = 10;
来源：http://hz.dianchejie.cn/gtfqgcydsf.html

[Q53] 按条件删除
来源：http://hz.gaohongyu789.top/gtfdsrajid.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shanyushiyangtech.top/gtumzpyfqd.html

[Q54] 清空表
来源：http://hz.yj20258.top/gtuwqizjhi.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigfzy.top/gtecqkwfsd.html

[Q55] 排名（并列占位）
来源：http://hz.zhixingplan.top/gtzirhpbsk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cucudq.cn/gtwsfnpnvx.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sysykeji.top/gtyxjveeph.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yuanzhike.top/gtiahhkuum.html

[Q57] 行号
来源：http://hz.wangshuangyany.cn/gtfduwquuy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jiagoushi.top/gtnlzjwqwk.html

[Q58] 累计求和
来源：http://hz.chenzaomai.com/gtjzvwtvtt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nwbrower.top/gtjbpjyzfz.html

[Q59] 分组内累计
来源：http://hz.daxiang520.top/gtdeoyzrnr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yanxiufei.cn/gtbirzrxnx.html

[Q60] 取上一行 / 下一行
来源：http://hz.svipenyu.cn/gtxoszudgv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.havefunace.top/gttuclgtea.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ybcxt.top/gtmdhnmjba.html

[Q61] 移动平均
来源：http://hz.fengsongda.top/gtpmryfnqb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zdqjudy.top/gtbdcjnfkt.html

[Q62] 分组占比
来源：http://hz.52xcode.cn/gtqnqybmem.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtfsxwhfos.html

[Q63] 开启事务
来源：http://hz.9152youxi.cn/gtafacamve.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ywan-chungtsiang.top/gtjmugiqvm.html

[Q64] 提交事务
来源：http://hz.zhengqikj.top/gtqzxiuzlq.html

COMMIT;
来源：http://hz.jlsjyb.cn/gtptvdzpxf.html

[Q65] 回滚事务
来源：http://hz.feifeiyinyue.top/gtyiztsrxz.html

ROLLBACK;
来源：http://hz.iojbl.cn/gtvuqghmer.html

[Q66] 行锁查询
来源：http://hz.nanxinkj.top/gtgiwhbigx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ehwqpu.com/gttrtwuozf.html

[Q67] 设置隔离级别
来源：http://hz.cucudq.cn/gtefczewmn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.quarkkingdee.top/gttkkslpxn.html

[Q68] 保存点
来源：http://hz.gaohongyu789.top/gtxoidgwxc.html

SAVEPOINT sp1;
来源：http://hz.chenjidiqi.icu/gtkukfzeig.html

ROLLBACK TO sp1;
来源：http://hz.jiagoushi.top/gtgyqxswok.html

[Q69] 查看执行计划
来源：http://hz.zhengqikj.top/gtxheeysgh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenzaomai.com/gtkozmaqud.html

[Q70] 更新统计信息
来源：http://hz.yueranfly.top/gtoarwfkfi.html

ANALYZE TABLE users;
来源：http://hz.jinyuanbaomall.cn/gtvobrflmm.html

[Q71] 查看建表语句
来源：http://hz.zhengqikj.top/gtkfrefgis.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ybcxt.top/gtifbbafzf.html

[Q72] 查看索引
来源：http://hz.smart0.xyz/gtgshfokka.html

SHOW INDEX FROM users;
来源：http://hz.cashguo.top/gtnshxzhjy.html

[Q73] 查看表状态
来源：http://hz.gaohongyu789.top/gtheldlgxo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hnqzz.top/gtfmvndkpx.html

[Q74] 强制使用索引
来源：http://hz.xziqi.cn/gtpeffvywu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jianghu66.top/gtdxmymboy.html

[Q75] 日期格式化
来源：http://hz.birdmap.top/gtlgskfjqo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hfpthk.cn/gtwpbqlkyv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cdnleiting.top/gtqknmnfyy.html

[Q76] 按天统计
来源：http://hz.jqgufenzy.top/gtbidqvnxc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhijiandao.cn/gtwtimviwm.html

[Q77] 时间加减
来源：http://hz.xuetiantiany.cn/gtokyagpeb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cheryme.top/gtmosqucza.html

[Q78] 当前时间
来源：http://hz.tanke756.top/gtsjslfcws.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ybcxt.top/gtwtpdgdsf.html

[Q79] 字符串拼接
来源：http://hz.daria6918.cn/gtpslnppse.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ydjk.org.cn/gtckdcyeio.html

[Q80] 字符串截取
来源：http://hz.zhongyouzk.top/gtxviuyyva.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.kuanghao11.cn/gtagcuqbvv.html

[Q81] 字符串替换
来源：http://hz.ivvv.top/gtsqqqoxkh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hfpthk.cn/gtjvywccvz.html

[Q82] 字符长度与字节长度
来源：http://hz.cqqwz.cn/gtzofkzjrc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj202588.top/gtaxenwotm.html

[Q83] 大小写转换
来源：http://hz.0kj1m.cn/gtasfrnonp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cucudq.cn/gtuujydseu.html

[Q84] 去除首尾空格
来源：http://hz.havefunace.top/gtvxcohpzk.html

SELECT TRIM(name) FROM users;
来源：http://hz.shanyushiyangtech.top/gtamwasvvv.html

[Q85] 数值取整
来源：http://hz.hnxiangtu.top/gtxvlouhmy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tianlin.xyz/gtyoolwyvm.html

[Q86] 读取 JSON 字段
来源：http://hz.cashguo.top/gthnguvdyp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hnxiangtu.top/gtntxbjmzt.html

[Q87] JSON 字段做条件
来源：http://hz.ivvv.top/gtjqtfmppm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.feifeiyinyue.top/gtjkgvnkjf.html

[Q88] 行转列（条件聚合）
来源：http://hz.guowangkeji.top/gtmpixqvtr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.chenjidiqi.icu/gtyiuzvvba.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.0kj1m.cn/gtxzwzlnim.html

[Q89] 判断表是否存在
来源：http://hz.nanxuanxn.top/gtlbgckvub.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yuanzhike.top/gttsdzzcsl.html

[Q90] 生成序号列
来源：http://hz.sysykeji.top/gtbfoilglb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ppjwa.cn/gtfeylvlbh.html

================================================================================
来源：http://hz.smart0.xyz/gtwzhozvdi.html

R. Bash 专题
来源：http://hz.xuanzx.com/gtzjcbaprx.html

================================================================================
来源：http://hz.nanxuanxn.top/gtvtgukpqw.html

[R01] shebang 与严格模式
来源：http://hz.hysaishi.cn/gtozrajrof.html

#!/usr/bin/env bash
来源：http://hz.daxiang520.top/gttdbhuldi.html

set -euo pipefail
来源：http://hz.vqdsnc.cn/gtpykqfzci.html

[R02] 变量赋值与使用
来源：http://hz.zhixingplan.top/gtzckxiyrk.html

name="Tom"; echo "$name"
来源：http://hz.jqgufenzy.top/gtpqosjrmw.html

[R03] 只读变量
来源：http://hz.ivvv.top/gtsaasddec.html

readonly PI=3.14
来源：http://hz.dianchejie.cn/gtultgggpd.html

[R04] 位置参数
来源：http://hz.yueranfly.top/gtevtyunrv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shzxlz.cn/gtkygumtxy.html

[R05] 参数默认值
来源：http://hz.chenzaomai.com/gttfyscqtm.html

name="${1:-default}"
来源：http://hz.haohaochexian.top/gtyexkasvc.html

[R06] 判断命令是否存在
来源：http://hz.yonumen.top/gtxqoxxrxe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nwbrower.top/gtegsikrzl.html

[R07] if 判断文件
来源：http://hz.chenjidiqi.icu/gtffmbgxup.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cucudq.cn/gtvcqlyjza.html

[R08] 数值比较
来源：http://hz.ehwqpu.com/gtayxfhfmg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.guowangkeji.top/gtnajmarxp.html

[R09] 字符串比较
来源：http://hz.gzhubu.top/gtxvfebpye.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xuanzx.com/gtfgkzlibx.html

[R10] 正则匹配
来源：http://hz.zhengqikj.top/gtnplmdnst.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.fzhhl.top/gtzemzpcix.html

[R11] case 多分支
来源：http://hz.cheryme.top/gtfjweyjmp.html

case "$1" in
来源：http://hz.snrcjt.cn/gtiyjhhocr.html

start) echo "启动" ;;
来源：http://hz.guannengcc.top/gtamqlnrbe.html

stop)  echo "停止" ;;
来源：http://hz.0kj1m.cn/gtkqytysbw.html

*)     echo "未知命令" ;;
来源：http://hz.nanxuanxn.top/gtaalqwjer.html

esac
来源：http://hz.jinqigufen.top/gtnsirsbxj.html

[R12] for 遍历文件
来源：http://hz.smart0.xyz/gtwfxagiol.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jianghu66.top/gtblertnyr.html

[R13] for 计数循环
来源：http://hz.jinqigufen.top/gtrhqwvaxn.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.52xcode.cn/gtpfssmbqj.html

[R14] C 风格 for
来源：http://hz.ppjwa.cn/gtieckmqlk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.birdmap.top/gtwgvjzbcn.html

[R15] while 逐行读文件
来源：http://hz.xinyue.icu/gtkedeqcag.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hongshengwenyu.top/gtmymyhxnn.html

[R16] until 等待条件
来源：http://hz.ydjk.org.cn/gtdqfrxcgl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hammf.cn/gtacefbuxi.html

[R17] 数组定义与取值
来源：http://hz.sysykeji.top/gtktzhknll.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ywan-chungtsiang.top/gtmxiulhys.html

[R18] 遍历数组
来源：http://hz.hywenlv.cn/gtqksbcjkj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fzhhl.top/gtxlvztixt.html

[R19] 数组长度
来源：http://hz.shuidangran.top/gtulkiarcn.html

echo "${#arr[@]}"
来源：http://hz.quarkkingdee.top/gtjjmcorvv.html

[R20] 关联数组（字典）
来源：http://hz.yongpay.top/gtzhvphhkq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.c1oappe.top/gtolyyecda.html

[R21] 字符串长度
来源：http://hz.hnxiangtu.top/gtdwomupze.html

echo "${#s}"
来源：http://hz.wangshuangyany.cn/gtfajskuhw.html

[R22] 截取子串
来源：http://hz.shuidangran.top/gtyeqkcxbi.html

echo "${s:0:5}"
来源：http://hz.haohaochexian.top/gtrdfidmku.html

[R23] 字符串替换
来源：http://hz.quarkkingdee.top/gtyikwfqpy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ydjk.org.cn/gtcjorferp.html

[R24] 大小写转换
来源：http://hz.chenjidiqi.icu/gtbqbnzcmq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258888.top/gtdkrqqdfo.html

[R25] 去后缀 / 去前缀
来源：http://hz.hnqzz.top/gtvnialyaf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.guannengcc.top/gtvfleidoj.html

[R26] 命令替换
来源：http://hz.zhaomingkeji.xyz/gtxmspvdko.html

now=$(date +%F); echo "$now"
来源：http://hz.hywenlv.cn/gtltnhmoze.html

[R27] 算术展开
来源：http://hz.bjfxy.top/gtnljwnaak.html

echo $((1 + 2 * 3))
来源：http://hz.ehwqpu.com/gtxmjsetpz.html

[R28] 浮点运算
来源：http://hz.mhx1999.top/gtnruykybr.html

echo "scale=2; 10/3" | bc
来源：http://hz.smart0.xyz/gtkwjaarse.html

[R29] 定义函数
来源：http://hz.yj20258888.top/gtzemaapss.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xuanzx.com/gtrdjcbmsx.html

[R30] 函数返回状态码
来源：http://hz.dianchejie.cn/gtkjzirqtt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jqgufenzy.top/gtzwxwvuuq.html

[R31] 局部变量
来源：http://hz.jqgufenzy.top/gtilxwgolb.html

f() { local x=1; echo "$x"; }
来源：http://hz.ywan-chungtsiang.top/gtzewxctyi.html

[R32] 参数个数校验
来源：http://hz.zdqjudy.top/gtdzpxaetq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj20258888.top/gtiqkxnapo.html

[R33] 捕获错误并提示行号
来源：http://hz.yj20258888.top/gtljbazklw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nwbrower.top/gtkgncrykr.html

[R34] 退出时清理
来源：http://hz.tianlin.xyz/gtpdtmlvig.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gthhrhized.html

[R35] 后台执行并等待
来源：http://hz.pycfn.com/gtireshlye.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.quarkkingdee.top/gtxgouzjxz.html

[R36] 并发执行多个任务
来源：http://hz.xingfuxueyuan.xyz/gtjfzoukqf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yueranfly.top/gtjekzwwzz.html

[R37] 把输出赋给变量
来源：http://hz.pengpengdd.cyou/gtqzqmyyui.html

files=$(ls -1)
来源：http://hz.zhaomingkeji.xyz/gtnfpdnbtm.html

[R38] 管道串联
来源：http://hz.yongpay.top/gtmbrgbgni.html

cat a.txt | grep -i error | wc -l
来源：http://hz.316326.xyz/gtuctwnvfp.html

[R39] 重定向标准输出与错误
来源：http://hz.zycfv.cn/gtyhqctwds.html

cmd > out.log 2>&1
来源：http://hz.daxiang520.top/gtmvbbdaev.html

[R40] 追加写日志
来源：http://hz.fzhhl.top/gtgvmldghg.html

echo "log" >> out.log
来源：http://hz.andypj.xyz/gtackuwsbt.html

[R41] 丢弃输出
来源：http://hz.jiagoushi.top/gtiwwbtjzo.html

cmd >/dev/null 2>&1
来源：http://hz.iojbl.cn/gtisdkyoxk.html

[R42] 输入重定向
来源：http://hz.redwolf501.top/gtbjawsoby.html

wc -l < a.txt
来源：http://hz.havefunace.top/gtzudfrgqk.html

[R43] 按名字查找文件
来源：http://hz.guannengcc.top/gtkknqjttn.html

find . -name "*.log" -type f
来源：http://hz.hnqzz.top/gtorwhgvef.html

[R44] 按修改时间查找
来源：http://hz.nwbrower.top/gtyiuuxeei.html

find . -mtime -7 -type f
来源：http://hz.ppjwa.cn/gtbljpcdos.html

[R45] 批量删除
来源：http://hz.andypj.xyz/gtahicfsgy.html

find . -name "*.tmp" -delete
来源：http://hz.svipenyu.cn/gtridarhgg.html

[R46] 递归替换文件内容
来源：http://hz.tian-w.cn/gtokbhnjvq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sweek.top/gtxpymjaai.html

[R47] sed 单行替换
来源：http://hz.cdnleiting.top/gtocrulpue.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.snrcjt.cn/gtwuroylna.html

[R48] awk 取指定列
来源：http://hz.fzhhl.top/gtnfrsjwmj.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinqigufen.top/gtbcpmcwrl.html

[R49] awk 带条件
来源：http://hz.guannengcc.top/gtwsgrpngn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shuidangran.top/gtsitdfpcq.html

[R50] awk 求和
来源：http://hz.52xcode.cn/gtndjruqup.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xylfe.cn/gtjulhlgzo.html

[R51] 排序去重取前几
来源：http://hz.mhx1999.top/gtiziowphj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.snrcjt.cn/gtambgmxec.html

[R52] 统计行数
来源：http://hz.jlsjyb.cn/gtgscesxpv.html

wc -l a.txt
来源：http://hz.yanxiufei.cn/gteqkwnjiz.html

[R53] 查看文件头与实时尾
来源：http://hz.sxryk.cn/gticqtelnu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hnqzz.top/gtvqywwamt.html

[R54] 比较两个文件
来源：http://hz.jinqigfzy.top/gtoqaxznwt.html

diff a.txt b.txt
来源：http://hz.yangfankeji.com/gtcbtwijqn.html

[R55] 压缩与解压
来源：http://hz.yj20258888.top/gtrnenjxol.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.redwolf501.top/gtfmzrjjdm.html

[R56] 远程拷贝
来源：http://hz.ehwqpu.com/gtxixbvgcq.html

scp file user@host:/path/
来源：http://hz.cheryme.top/gtvlfzoixv.html

[R57] 远程执行命令
来源：http://hz.yongpay.top/gtebijzqxj.html

ssh user@host 'uptime'
来源：http://hz.ydzc1.top/gtircfeulc.html

[R58] 下载文件
来源：http://hz.chenzaomai.com/gtzninfbek.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xinyue.icu/gtvwplgazn.html

[R59] 发 POST JSON
来源：http://hz.guannengcc.top/gtlnthjlzv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.wangshuangyany.cn/gtklelqnms.html

[R60] 只看 HTTP 状态码
来源：http://hz.jiagoushi.top/gtwohjxbsu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ivvv.top/gtxotoacrj.html

[R61] 磁盘占用
来源：http://hz.xuetiantiany.cn/gtvvzphzxr.html

df -h;  du -sh *
来源：http://hz.shangyingyoupin.top/gtxqjnhvbc.html

[R62] 找最占空间的文件
来源：http://hz.cucudq.cn/gtkxmekjmx.html

du -ah . | sort -rh | head -10
来源：http://hz.jinqigufen.top/gtlalzxvmu.html

[R63] 内存与进程
来源：http://hz.hfpthk.cn/gtcsvigcqv.html

free -h;  ps aux | grep nginx
来源：http://hz.zhixingplan.top/gtymfijvvf.html

[R64] 结束进程
来源：http://hz.guannengcc.top/gtnjfwbrsk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ivvv.top/gtqhcqvsff.html

[R65] 查看端口占用
来源：http://hz.dianchejie.cn/gtqwqghkgg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.daria6918.cn/gtjxxlrjrm.html

[R66] 定时任务
来源：http://hz.jqgufenzy.top/gtbatiijik.html

crontab -e;  crontab -l
来源：http://hz.ehwqpu.com/gtatyffqir.html

[R67] 生成随机十六进制串
来源：http://hz.ppjwa.cn/gtxwrrflor.html

openssl rand -hex 16
来源：http://hz.hnqzz.top/gtggfihbzi.html

[R68] 计算文件校验值
来源：http://hz.jqgfzy.top/gtmnhldvqv.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jqgfzy.top/gtgchzdkcs.html

[R69] 生成随机密码
来源：http://hz.aibaodan.cn/gtjgzcymhi.html

head -c 16 /dev/urandom | base64
来源：http://hz.zycfv.cn/gtwxjjrens.html

[R70] 时间戳与互转
来源：http://hz.yueranfly.top/gtsxvdtmit.html

date +%s;  date -d @1700000000
来源：http://hz.vqdsnc.cn/gtxstnabfg.html

[R71] 日期格式化
来源：http://hz.redwolf501.top/gtxrfonerl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nanxuanxn.top/gtqctecfpv.html

[R72] 等待端口就绪
来源：http://hz.haohaochexian.top/gtdioyhydg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cucudq.cn/gtakgypufn.html

[R73] 分割大日志
来源：http://hz.aizwys.cn/gtisflxjfh.html

split -l 1000 big.log part_
来源：http://hz.yj20258.top/gtkzovfgoj.html

[R74] 批量重命名
来源：http://hz.sxryk.cn/gtkggezjtb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zycfv.cn/gthnepcoeu.html

[R75] 导出环境变量
来源：http://hz.kuanghao11.cn/gtjydlntnp.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gzhubu.top/gtwqbnoyux.html

[R76] 使用临时文件
来源：http://hz.jiagoushi.top/gtyykmterh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258888.top/gtfppzjikn.html

[R77] 读取用户输入
来源：http://hz.chenjidiqi.icu/gtsmrjoxej.html

read -rp "请输入: " ans
来源：http://hz.shangyingyoupin.top/gtgxjsjsvr.html

[R78] 交互式菜单
来源：http://hz.sxryk.cn/gtphntltyx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xinyue.icu/gtudgwugum.html

[R79] 解析命令行选项
来源：http://hz.cucudq.cn/gtqvyjqouk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yongpay.top/gtazdlmhiu.html

[R80] 查看脚本执行耗时
来源：http://hz.ivvv.top/gthfpyfrgl.html

time ./run.sh
来源：http://hz.ydzc1.top/gtoidwbphz.html

================================================================================
来源：http://hz.ehwqpu.com/gtndxmdqlo.html


<!-- 参考信息 -->