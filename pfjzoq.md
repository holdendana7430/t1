代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shangyingyoupin.top/gtaorxooqh.html

[Q30] 分组统计
来源：http://hz.tian-w.cn/gtqdomlfap.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinqigufen.top/gtzipwapax.html

[Q31] 分组后过滤
来源：http://hz.zycfv.cn/gttenqzmma.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.0kj1m.cn/gtkpxpraap.html

[Q32] 分组拼接字符串
来源：http://hz.nwbrower.top/gtjkovuqam.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jqgufenzy.top/gteqxauuan.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.dashuyun.cn/gtdnihpezx.html

[Q33] 多列分组
来源：http://hz.nanxuanxn.top/gtwdqeerbs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yueranfly.top/gtasnubhas.html

[Q34] 每组取第一条
来源：http://hz.cashguo.top/gtimmrjtzo.html

SELECT * FROM (
来源：http://hz.birdmap.top/gtjilvxetp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.9152youxi.cn/gtxkigiokz.html

) t WHERE rn = 1;
来源：http://hz.9152youxi.cn/gtnqzxsxup.html

[Q35] 内连接
来源：http://hz.tian-w.cn/gttrwqozbm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhiwuduotai.top/gtilckkzsp.html

[Q36] 左连接
来源：http://hz.cucudq.cn/gtpofqdtyh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.9152youxi.cn/gtssxmylht.html

[Q37] 右连接
来源：http://hz.316326.xyz/gtzqxszgdm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yuxming.cn/gtypumvllq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.snrcjt.cn/gtzjvhgdcx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.snrcjt.cn/gtcrjuwagh.html

[Q39] 自连接（查上下级）
来源：http://hz.dashuyun.cn/gtzxkmifxy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xylfe.cn/gtokbbvpbr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhoulong.xyz/gtmwixuoub.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhoulong.xyz/gtlxqqqobz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zycfv.cn/gtcgvhdsdb.html

[Q41] 多表连接
来源：http://hz.zhoulong.xyz/gtnicqvmqt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhaomingkeji.xyz/gthylgddjy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.nanxuanxn.top/gttyxniigi.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhaomingkeji.xyz/gtpnnuavuk.html

[Q42] 连接条件附加过滤
来源：http://hz.52xcode.cn/gtbdoqctbb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.kuanghao11.cn/gtcfaurbnd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yueranfly.top/gtrfszmmzl.html

[Q43] 标量子查询
来源：http://hz.cdnleiting.top/gtemwactvb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.aizwys.cn/gtwnymyryf.html

[Q44] IN 子查询
来源：http://hz.zhijiandao.cn/gtmjghalgg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gaohongyu789.top/gtfelbhitp.html

[Q45] EXISTS 判断存在
来源：http://hz.cqqwz.cn/gtudrnkjfr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pengpengdd.cyou/gtrcgmlciq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.chenlongwang.top/gtrghbxkbp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guowangkeji.top/gtkmovhwxr.html

[Q47] 与平均值比较
来源：http://hz.hywenlv.cn/gtmaoehxfo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ydzc1.top/gtbwfkgtlm.html

[Q48] CTE 公用表表达式
来源：http://hz.yj202588.top/gtbajksdrq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jiagoushi.top/gtovorszod.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj20258.top/gtzedpfyxa.html

[Q49] 更新单行
来源：http://hz.jqgfzy.top/gtmucbzopl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.dianchejie.cn/gtdterwscg.html

[Q50] 批量更新
来源：http://hz.ybcxt.top/gtvdjrdhoi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yangfankeji.com/gtzjuhoftf.html

[Q51] 用子查询更新
来源：http://hz.hongshengwenyu.top/gttwznhcmg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jianghu66.top/gtgrgokgxs.html

[Q52] 删除指定行
来源：http://hz.jiagoushi.top/gtsbkxjmoy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.svipenyu.cn/gtcypjblrm.html

[Q53] 按条件删除
来源：http://hz.jyoumei.cn/gtkgjphlzr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.guowangkeji.top/gtotzwaggz.html

[Q54] 清空表
来源：http://hz.chenjidiqi.icu/gtcpyuidxv.html

TRUNCATE TABLE logs;
来源：http://hz.haohaochexian.top/gtqxuhfatx.html

[Q55] 排名（并列占位）
来源：http://hz.xinyue.icu/gtredfvomj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.havefunace.top/gtapzlhrri.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ehwqpu.com/gtnibgsnoj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.iojbl.cn/gtunqqblba.html

[Q57] 行号
来源：http://hz.cdnleiting.top/gtxvpggdml.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.tianlin.xyz/gtbytjvroe.html

[Q58] 累计求和
来源：http://hz.daxiang520.top/gtveiacwxb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhoulong.xyz/gtledypdor.html

[Q59] 分组内累计
来源：http://hz.hongshengwenyu.top/gtbmhetlzw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ybcxt.top/gtfibtdlei.html

[Q60] 取上一行 / 下一行
来源：http://hz.xinyue.icu/gtcfhpmkbf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.nanxinkj.top/gtdcgrhsow.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.pengpengdd.cyou/gtxuinuejp.html

[Q61] 移动平均
来源：http://hz.fzhhl.top/gtjaaxbnut.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgufenzy.top/gtznprjvjm.html

[Q62] 分组占比
来源：http://hz.cdnleiting.top/gtvaxoqhxy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtcmqdpwqc.html

[Q63] 开启事务
来源：http://hz.mhx1999.top/gtvvrfqkpz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cashguo.top/gtaqhafuoz.html

[Q64] 提交事务
来源：http://hz.gaohongyu789.top/gtfsoniqul.html

COMMIT;
来源：http://hz.yueranfly.top/gtrbtwvmiz.html

[Q65] 回滚事务
来源：http://hz.fzhhl.top/gtufmjmmtb.html

ROLLBACK;
来源：http://hz.hysaishi.cn/gtdmxhlnxq.html

[Q66] 行锁查询
来源：http://hz.havefunace.top/gtnkeqowcc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.52xcode.cn/gtpwocanyo.html

[Q67] 设置隔离级别
来源：http://hz.jqgfzy.top/gtwdxrpwwq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shuidangran.top/gtlkditndi.html

[Q68] 保存点
来源：http://hz.zhengqikj.top/gtdkwudblh.html

SAVEPOINT sp1;
来源：http://hz.daxiang520.top/gtbfrqetka.html

ROLLBACK TO sp1;
来源：http://hz.hfpthk.cn/gtykidbbil.html

[Q69] 查看执行计划
来源：http://hz.ydzc1.top/gtbcccwdkb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.snrcjt.cn/gtfcrtgxmg.html

[Q70] 更新统计信息
来源：http://hz.jinyuanbaomall.cn/gtuwrdidev.html

ANALYZE TABLE users;
来源：http://hz.ehwqpu.com/gtlbuwotjq.html

[Q71] 查看建表语句
来源：http://hz.sufxvd.cn/gtpfgcgkjy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.mhx1999.top/gtxyjqhbzt.html

[Q72] 查看索引
来源：http://hz.xylfe.cn/gtyhihfnig.html

SHOW INDEX FROM users;
来源：http://hz.zhaomingkeji.xyz/gtzkdtovbm.html

[Q73] 查看表状态
来源：http://hz.yanxiufei.cn/gtnqbmsgjb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.dianchejie.cn/gtdlgftxyj.html

[Q74] 强制使用索引
来源：http://hz.jlsjyb.cn/gtfafhdxgi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yonumen.top/gtjchmlyqr.html

[Q75] 日期格式化
来源：http://hz.yanxiufei.cn/gtuxwxsbiy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.dianchejie.cn/gtmdythpzk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sysykeji.top/gtrnwzxwcl.html

[Q76] 按天统计
来源：http://hz.zhengqikj.top/gtansickfq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hnxiangtu.top/gtgvajddof.html

[Q77] 时间加减
来源：http://hz.jiagoushi.top/gtbynpfoaz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jyoumei.cn/gtqmkegeeo.html

[Q78] 当前时间
来源：http://hz.svipenyu.cn/gtctecvokb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yuanzhike.top/gtawobbqqq.html

[Q79] 字符串拼接
来源：http://hz.redwolf501.top/gtpcmmcter.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj202588.top/gtngzemoca.html

[Q80] 字符串截取
来源：http://hz.jinqigfzy.top/gtijalaqba.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.bjfxy.top/gtvtotitbn.html

[Q81] 字符串替换
来源：http://hz.yj20258888.top/gteyrsfedi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yanxiufei.cn/gtisqsazyy.html

[Q82] 字符长度与字节长度
来源：http://hz.xziqi.cn/gtxfgqzzvk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cheryme.top/gtozqwmiac.html

[Q83] 大小写转换
来源：http://hz.wangdashe.top/gtnrkdoxos.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jianghu66.top/gtmxyzufhz.html

[Q84] 去除首尾空格
来源：http://hz.52xcode.cn/gtjwkktwrk.html

SELECT TRIM(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtiiaxjssh.html

[Q85] 数值取整
来源：http://hz.daxiang520.top/gtpgbculgf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hysaishi.cn/gtbmkwwtls.html

[Q86] 读取 JSON 字段
来源：http://hz.nwbrower.top/gttoryjbwy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258.top/gtomiovlva.html

[Q87] JSON 字段做条件
来源：http://hz.gotoacloud.top/gtubiszecb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.pycfn.com/gtydrrtfco.html

[Q88] 行转列（条件聚合）
来源：http://hz.hywenlv.cn/gtahpgppvw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jianghu66.top/gtoyaypunp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gotoacloud.top/gtvxktnuho.html

[Q89] 判断表是否存在
来源：http://hz.hfpthk.cn/gtylpmtbuv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhiwuduotai.top/gtpyonlgip.html

[Q90] 生成序号列
来源：http://hz.cqqwz.cn/gtnvmqqryj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ivvv.top/gtynhohhqr.html

================================================================================
来源：http://hz.guowangkeji.top/gtfnyzdjuy.html

R. Bash 专题
来源：http://hz.nanxinkj.top/gtfyphbxmk.html

================================================================================
来源：http://hz.nanxuanxn.top/gtzncvapzo.html

[R01] shebang 与严格模式
来源：http://hz.xinyue.icu/gtbinzllpm.html

#!/usr/bin/env bash
来源：http://hz.pengpengdd.cyou/gtwocgxkly.html

set -euo pipefail
来源：http://hz.pengpengdd.cyou/gtfpasmpak.html

[R02] 变量赋值与使用
来源：http://hz.nwbrower.top/gtgkgssuuz.html

name="Tom"; echo "$name"
来源：http://hz.cdnleiting.top/gtjixzdywy.html

[R03] 只读变量
来源：http://hz.tian-w.cn/gtfkcwfyzu.html

readonly PI=3.14
来源：http://hz.xylfe.cn/gtilhidbzz.html

[R04] 位置参数
来源：http://hz.xinyue.icu/gtkrtbxyfp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cdnleiting.top/gtsqfvpsbx.html

[R05] 参数默认值
来源：http://hz.quarkkingdee.top/gtccabhchh.html

name="${1:-default}"
来源：http://hz.ppjwa.cn/gtoigcderx.html

[R06] 判断命令是否存在
来源：http://hz.hnqzz.top/gtoxibxarj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinqigfzy.top/gtcoyrwjmq.html

[R07] if 判断文件
来源：http://hz.hongshengwenyu.top/gtnhrwshja.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xinyue.icu/gtwduarxkq.html

[R08] 数值比较
来源：http://hz.dashuyun.cn/gtppbfekin.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shzxlz.cn/gtdkxmopug.html

[R09] 字符串比较
来源：http://hz.feifeiyinyue.top/gtqalkrwvk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.kuanghao11.cn/gtlxaaaeok.html

[R10] 正则匹配
来源：http://hz.shangyingyoupin.top/gtkacvspuc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.guannengcc.top/gtnzhgfvml.html

[R11] case 多分支
来源：http://hz.xinyue.icu/gtcubtglel.html

case "$1" in
来源：http://hz.dashuyun.cn/gtfizhljty.html

start) echo "启动" ;;
来源：http://hz.redwolf501.top/gtpsylauby.html

stop)  echo "停止" ;;
来源：http://hz.zycfv.cn/gthxajvdni.html

*)     echo "未知命令" ;;
来源：http://hz.zhixingplan.top/gtdphfbuxd.html

esac
来源：http://hz.nanxinkj.top/gtzkhthtky.html

[R12] for 遍历文件
来源：http://hz.jyoumei.cn/gtjqyfjqef.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cqqwz.cn/gtpypexcna.html

[R13] for 计数循环
来源：http://hz.yanxiufei.cn/gtcxsdmuod.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jianghu66.top/gtfdmqqlmm.html

[R14] C 风格 for
来源：http://hz.haohaochexian.top/gtbbqjjndl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zycfv.cn/gtsaznmdqz.html

[R15] while 逐行读文件
来源：http://hz.pycfn.com/gteanrgjvx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shanyushiyangkeji.top/gtfpyainkd.html

[R16] until 等待条件
来源：http://hz.iojbl.cn/gtuzlrenoc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.andypj.xyz/gtfbcfgvus.html

[R17] 数组定义与取值
来源：http://hz.yj20258.top/gtrtyqzxsy.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenlongwang.top/gtmadaowqi.html

[R18] 遍历数组
来源：http://hz.svipenyu.cn/gtxiphuqbw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinghuilouyu.cn/gtlecjuecn.html

[R19] 数组长度
来源：http://hz.cqqwz.cn/gtcrxzjjdx.html

echo "${#arr[@]}"
来源：http://hz.chenjidiqi.icu/gtxftxsmka.html

[R20] 关联数组（字典）
来源：http://hz.birdmap.top/gtongvtakf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hnxiangtu.top/gtxdvufvag.html

[R21] 字符串长度
来源：http://hz.xuetiantiany.cn/gtvbwhfbgv.html

echo "${#s}"
来源：http://hz.jinqigfzy.top/gtzivgwyuw.html

[R22] 截取子串
来源：http://hz.redwolf501.top/gtxgolojig.html

echo "${s:0:5}"
来源：http://hz.pengpengdd.cyou/gtbqfsjxyp.html

[R23] 字符串替换
来源：http://hz.xuetiantiany.cn/gtmfcjhiwd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sufxvd.cn/gtqyzvrfjd.html

[R24] 大小写转换
来源：http://hz.jiagoushi.top/gturbrttfl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.52xcode.cn/gtolzbhwov.html

[R25] 去后缀 / 去前缀
来源：http://hz.aizwys.cn/gtjkspvjru.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xinyue.icu/gtsgzhvtqr.html

[R26] 命令替换
来源：http://hz.jlsjyb.cn/gtxtdmqwyu.html

now=$(date +%F); echo "$now"
来源：http://hz.yongpay.top/gtuyccpqkj.html

[R27] 算术展开
来源：http://hz.daxiang520.top/gtvitqbakp.html

echo $((1 + 2 * 3))
来源：http://hz.yj202588.top/gtbqprxfyq.html

[R28] 浮点运算
来源：http://hz.xingfuxueyuan.xyz/gtohudurbm.html

echo "scale=2; 10/3" | bc
来源：http://hz.hongshengwenyu.top/gtalydyczn.html

[R29] 定义函数
来源：http://hz.smart0.xyz/gttxjsmgni.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.bjfxy.top/gtfovvdozh.html

[R30] 函数返回状态码
来源：http://hz.smart0.xyz/gtugmsuply.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gzhubu.top/gtfilnruem.html

[R31] 局部变量
来源：http://hz.yueranfly.top/gtetfnmijp.html

f() { local x=1; echo "$x"; }
来源：http://hz.pycfn.com/gtpjqnwxto.html

[R32] 参数个数校验
来源：http://hz.hywenlv.cn/gtasnipbrp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxuanxn.top/gtvueivaic.html

[R33] 捕获错误并提示行号
来源：http://hz.ydjk.org.cn/gtfogkjbuc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.guannengcc.top/gtmhwicfwr.html

[R34] 退出时清理
来源：http://hz.nanxuanxn.top/gtcpqboaum.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yangfankeji.com/gtbuzthuci.html

[R35] 后台执行并等待
来源：http://hz.sufxvd.cn/gtnsnvgcbr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj20258888.top/gtbsnwyqyr.html

[R36] 并发执行多个任务
来源：http://hz.daria6918.cn/gtwiylchyc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cheryme.top/gthytojlnd.html

[R37] 把输出赋给变量
来源：http://hz.tianlin.xyz/gtzstgelvy.html

files=$(ls -1)
来源：http://hz.zhongyouzk.top/gtvkjcamqf.html

[R38] 管道串联
来源：http://hz.daxiang520.top/gtuyquxgfa.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinqigfzy.top/gtigqamhxq.html

[R39] 重定向标准输出与错误
来源：http://hz.dashuyun.cn/gtnurcknzf.html

cmd > out.log 2>&1
来源：http://hz.gogol.net.cn/gtijfkigjt.html

[R40] 追加写日志
来源：http://hz.hfpthk.cn/gtbofqweyr.html

echo "log" >> out.log
来源：http://hz.hnxiangtu.top/gtimcypkov.html

[R41] 丢弃输出
来源：http://hz.vqdsnc.cn/gtabtdkmfd.html

cmd >/dev/null 2>&1
来源：http://hz.hammf.cn/gtxcvtsqec.html

[R42] 输入重定向
来源：http://hz.jianghu66.top/gtgqjlvtlo.html

wc -l < a.txt
来源：http://hz.ppjwa.cn/gtaskfbfkx.html

[R43] 按名字查找文件
来源：http://hz.316326.xyz/gtnjyvcbxq.html

find . -name "*.log" -type f
来源：http://hz.nwbrower.top/gtzwkhmffl.html

[R44] 按修改时间查找
来源：http://hz.jqgfzy.top/gttzvrbyvj.html

find . -mtime -7 -type f
来源：http://hz.cheryme.top/gtobvyajdr.html

[R45] 批量删除
来源：http://hz.jinyuanbaomall.cn/gtxnqqamww.html

find . -name "*.tmp" -delete
来源：http://hz.yonumen.top/gtxaekvexf.html

[R46] 递归替换文件内容
来源：http://hz.yongpay.top/gtdcjgcbsc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cqqwz.cn/gtlfizxgfa.html

[R47] sed 单行替换
来源：http://hz.daria6918.cn/gtaxheussn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sxryk.cn/gtnkhvstmb.html

[R48] awk 取指定列
来源：http://hz.daria6918.cn/gtnysoipsk.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhaomingkeji.xyz/gtqbwvllyq.html

[R49] awk 带条件
来源：http://hz.hongshengwenyu.top/gtptigirgs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yuxming.cn/gtnbzaztac.html

[R50] awk 求和
来源：http://hz.xylfe.cn/gtlqhqtzcc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hammf.cn/gtpelvywum.html

[R51] 排序去重取前几
来源：http://hz.hammf.cn/gtbgkczygi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydzc1.top/gtlwyzekbq.html

[R52] 统计行数
来源：http://hz.316326.xyz/gtsoeqoirt.html

wc -l a.txt
来源：http://hz.guannengcc.top/gtqfdhaltg.html

[R53] 查看文件头与实时尾
来源：http://hz.tian-w.cn/gtpxvbwkhw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.0kj1m.cn/gtefklmfjy.html

[R54] 比较两个文件
来源：http://hz.aizwys.cn/gtywkfamly.html

diff a.txt b.txt
来源：http://hz.yvedp.cn/gtfjgconco.html

[R55] 压缩与解压
来源：http://hz.gotoacloud.top/gtkoibqcrd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zycfv.cn/gtqtridrzv.html

[R56] 远程拷贝
来源：http://hz.dianchejie.cn/gtcbiwqifz.html

scp file user@host:/path/
来源：http://hz.fengsongda.top/gtysmjcphi.html

[R57] 远程执行命令
来源：http://hz.xingfuxueyuan.xyz/gtohszderk.html

ssh user@host 'uptime'
来源：http://hz.gotoacloud.top/gtonhffcea.html

[R58] 下载文件
来源：http://hz.chenzaomai.com/gtavydmpbv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.quarkkingdee.top/gtefzkijvl.html

[R59] 发 POST JSON
来源：http://hz.chenlongwang.top/gtnpxpsevd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yanxiufei.cn/gtjjbitewu.html

[R60] 只看 HTTP 状态码
来源：http://hz.tian-w.cn/gtkkkuquyu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hywenlv.cn/gtierfntkb.html

[R61] 磁盘占用
来源：http://hz.yueranfly.top/gtcymbzhbw.html

df -h;  du -sh *
来源：http://hz.wangshuangyany.cn/gtkydxzjpm.html

[R62] 找最占空间的文件
来源：http://hz.hfpthk.cn/gtekrlzksh.html

du -ah . | sort -rh | head -10
来源：http://hz.ydjk.org.cn/gtakblsupd.html

[R63] 内存与进程
来源：http://hz.yj20258.top/gtqitoebit.html

free -h;  ps aux | grep nginx
来源：http://hz.gzhubu.top/gtlnxhumjx.html

[R64] 结束进程
来源：http://hz.nanxinkj.top/gtexjgcwao.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenzaomai.com/gtfmiurasi.html

[R65] 查看端口占用
来源：http://hz.sysykeji.top/gtzyqsahdi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ydjk.org.cn/gtgjiqclxx.html

[R66] 定时任务
来源：http://hz.pycfn.com/gthylxeuui.html

crontab -e;  crontab -l
来源：http://hz.chenjidiqi.icu/gtsqydxdjy.html

[R67] 生成随机十六进制串
来源：http://hz.dianchejie.cn/gtosyyvhpk.html

openssl rand -hex 16
来源：http://hz.yanxiufei.cn/gtjtweelli.html

[R68] 计算文件校验值
来源：http://hz.zhaomingkeji.xyz/gtnozyfuso.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.mhx1999.top/gteqheemkq.html

[R69] 生成随机密码
来源：http://hz.jianghu66.top/gtzpnoieok.html

head -c 16 /dev/urandom | base64
来源：http://hz.hongshengwenyu.top/gtsmrrgymy.html

[R70] 时间戳与互转
来源：http://hz.yueranfly.top/gtiznkmpkt.html

date +%s;  date -d @1700000000
来源：http://hz.cucudq.cn/gtexgwjyle.html

[R71] 日期格式化
来源：http://hz.zhongyouzk.top/gtatjokosh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cheryme.top/gtlsdscfjq.html

[R72] 等待端口就绪
来源：http://hz.ppjwa.cn/gtyjqruzws.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cheryme.top/gtmcrivjbu.html

[R73] 分割大日志
来源：http://hz.nanxinkj.top/gthheemmer.html

split -l 1000 big.log part_
来源：http://hz.ydzc1.top/gtmpowfnti.html

[R74] 批量重命名
来源：http://hz.pengpengdd.cyou/gtngasafai.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sxryk.cn/gtibiogciv.html

[R75] 导出环境变量
来源：http://hz.xinyue.icu/gtqwgeldkr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xingfuxueyuan.xyz/gtjwqcdhhd.html

[R76] 使用临时文件
来源：http://hz.yueranfly.top/gtutruwgrz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.0kj1m.cn/gtozecaprz.html

[R77] 读取用户输入
来源：http://hz.yuxming.cn/gtnbpnmzir.html

read -rp "请输入: " ans
来源：http://hz.guowangkeji.top/gtrnucoitf.html

[R78] 交互式菜单
来源：http://hz.yueranfly.top/gtoeurqyeq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jqgfzy.top/gtjmlrqkbg.html

[R79] 解析命令行选项
来源：http://hz.birdmap.top/gtixzxkdyg.html


<!-- 参考信息 -->