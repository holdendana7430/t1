代发 wailian999

[Q33] 多列分组
来源：http://hz.smart0.xyz/gtfijeqwfz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ppjwa.cn/gtiwfmammm.html

[Q34] 每组取第一条
来源：http://hz.ivvv.top/gtxtvnfcgh.html

SELECT * FROM (
来源：http://hz.zhongyouzk.top/gttkamvnsy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xingfuxueyuan.xyz/gtglnbnewp.html

) t WHERE rn = 1;
来源：http://hz.yanxiufei.cn/gthayikeoa.html

[Q35] 内连接
来源：http://hz.gaohongyu789.top/gtsxmtlupn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuanzx.com/gtlgvjsytv.html

[Q36] 左连接
来源：http://hz.yonumen.top/gtnmutvukx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.aizwys.cn/gtkcvjeyqx.html

[Q37] 右连接
来源：http://hz.tian-w.cn/gtvqbqqxac.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhoulong.xyz/gtktgvkubs.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cashguo.top/gtpoptbpuk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.dianchejie.cn/gtfvwynydo.html

[Q39] 自连接（查上下级）
来源：http://hz.ydzc1.top/gtzamrmyvy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ywan-chungtsiang.top/gtfhwamdul.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shanyushiyangtech.top/gtujkovwgu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gzhubu.top/gtknlosfnm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cucudq.cn/gtmzjmwvmg.html

[Q41] 多表连接
来源：http://hz.316326.xyz/gtgtlboemn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.chenzaomai.com/gtrkrzlhwm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.nwbrower.top/gtlfrryzbk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.havefunace.top/gtxtwnqgnd.html

[Q42] 连接条件附加过滤
来源：http://hz.316326.xyz/gtlircgfie.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tanke756.top/gtequlrbry.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yongpay.top/gtxaqxwkgh.html

[Q43] 标量子查询
来源：http://hz.zhongyouzk.top/gttyeygnbl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ehwqpu.com/gthksvajly.html

[Q44] IN 子查询
来源：http://hz.snrcjt.cn/gtguxqhprx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ivvv.top/gteipctzva.html

[Q45] EXISTS 判断存在
来源：http://hz.guowangkeji.top/gtjoiqgrod.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.svipenyu.cn/gtpoxrmhwy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cqqwz.cn/gtiijdxgmx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zycfv.cn/gteisjshsk.html

[Q47] 与平均值比较
来源：http://hz.quarkkingdee.top/gtatlweqia.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shzxlz.cn/gtdwdygsyz.html

[Q48] CTE 公用表表达式
来源：http://hz.jlsjyb.cn/gtxzmdbjxz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.sweek.top/gtzjtdikqh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ivvv.top/gtqzkyubid.html

[Q49] 更新单行
来源：http://hz.jyoumei.cn/gtsnyaoyqz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cdnleiting.top/gteisegbyw.html

[Q50] 批量更新
来源：http://hz.jinyuanbaomall.cn/gtudhsqnxk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zycfv.cn/gtducpusos.html

[Q51] 用子查询更新
来源：http://hz.jqgfzy.top/gtlhkwnvzo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.haohaochexian.top/gtxnkfyylo.html

[Q52] 删除指定行
来源：http://hz.yj20258888.top/gtajkqjuwk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.kuanghao11.cn/gttmjkirvq.html

[Q53] 按条件删除
来源：http://hz.bjfxy.top/gtuxfustka.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.0kj1m.cn/gtkyccvfve.html

[Q54] 清空表
来源：http://hz.jqgfzy.top/gtxosavsqm.html

TRUNCATE TABLE logs;
来源：http://hz.gaohongyu789.top/gtvkjgkutq.html

[Q55] 排名（并列占位）
来源：http://hz.bjfxy.top/gtqnuzpemf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ywan-chungtsiang.top/gtzlepzebg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hfpthk.cn/gtejqxtnay.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xylfe.cn/gtccdfwsxo.html

[Q57] 行号
来源：http://hz.9152youxi.cn/gtfjbihgdc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yonumen.top/gtpvpkqrrb.html

[Q58] 累计求和
来源：http://hz.daxiang520.top/gtlgbsocsh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shuidangran.top/gtvdondhap.html

[Q59] 分组内累计
来源：http://hz.jlsjyb.cn/gtltdsoxcx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gthwikrraa.html

[Q60] 取上一行 / 下一行
来源：http://hz.sysykeji.top/gtejecvzed.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shzxlz.cn/gtzvvsoxfz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.daria6918.cn/gtwrndjhao.html

[Q61] 移动平均
来源：http://hz.mhx1999.top/gtpsqhhnyb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shanyushiyangtech.top/gtobvmhekk.html

[Q62] 分组占比
来源：http://hz.sysykeji.top/gtglcruhhx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gtpuzruvzq.html

[Q63] 开启事务
来源：http://hz.jyoumei.cn/gtisspnkvw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hammf.cn/gtrictosko.html

[Q64] 提交事务
来源：http://hz.hfpthk.cn/gtcuvewrzj.html

COMMIT;
来源：http://hz.xuetiantiany.cn/gtoojajtmj.html

[Q65] 回滚事务
来源：http://hz.yongpay.top/gtpbnceevd.html

ROLLBACK;
来源：http://hz.jinqigfzy.top/gtcxdluwtg.html

[Q66] 行锁查询
来源：http://hz.hnxiangtu.top/gtpnxfaptb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenlongwang.top/gtywmaxinj.html

[Q67] 设置隔离级别
来源：http://hz.hysaishi.cn/gtefaxkmbk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhixingplan.top/gtdhaovdpg.html

[Q68] 保存点
来源：http://hz.nanxuanxn.top/gtfpwnudbr.html

SAVEPOINT sp1;
来源：http://hz.ydzc1.top/gthvrwkuqa.html

ROLLBACK TO sp1;
来源：http://hz.cheryme.top/gthlojetgn.html

[Q69] 查看执行计划
来源：http://hz.andypj.xyz/gtrdpfaryo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ivvv.top/gtmwruleal.html

[Q70] 更新统计信息
来源：http://hz.havefunace.top/gtmtmbaggx.html

ANALYZE TABLE users;
来源：http://hz.yongpay.top/gtfcscgckt.html

[Q71] 查看建表语句
来源：http://hz.hnqzz.top/gtfopbxucn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hywenlv.cn/gtinaqjqyj.html

[Q72] 查看索引
来源：http://hz.hnxiangtu.top/gtnsbjcymp.html

SHOW INDEX FROM users;
来源：http://hz.dianchejie.cn/gtgumnoirt.html

[Q73] 查看表状态
来源：http://hz.hywenlv.cn/gtazsxkubq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.iojbl.cn/gteymtaidz.html

[Q74] 强制使用索引
来源：http://hz.smart0.xyz/gtvenuatbn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sweek.top/gtbnkanuxr.html

[Q75] 日期格式化
来源：http://hz.nanxinkj.top/gtvwoorfie.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.guannengcc.top/gtrxcvkeve.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.redwolf501.top/gtwpcysybd.html

[Q76] 按天统计
来源：http://hz.yvedp.cn/gtbrrjvsiq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ivvv.top/gtxlpjzqcz.html

[Q77] 时间加减
来源：http://hz.guannengcc.top/gtkmaqzxkn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yj20258.top/gtvtwdswwe.html

[Q78] 当前时间
来源：http://hz.shzxlz.cn/gtdmrsxjns.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sysykeji.top/gthvbniexu.html

[Q79] 字符串拼接
来源：http://hz.zhongyouzk.top/gtiljxdzvf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.meibo888.top/gtiiobmiot.html

[Q80] 字符串截取
来源：http://hz.vqdsnc.cn/gtaqvnlwik.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cdnleiting.top/gtwequefhu.html

[Q81] 字符串替换
来源：http://hz.sysykeji.top/gtjatiogsc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenzaomai.com/gtmfkxpdte.html

[Q82] 字符长度与字节长度
来源：http://hz.dashuyun.cn/gtczokibwv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fengsongda.top/gtpydnhjji.html

[Q83] 大小写转换
来源：http://hz.havefunace.top/gtaucxwjoe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jiagoushi.top/gtdffxdtys.html

[Q84] 去除首尾空格
来源：http://hz.hnxiangtu.top/gtlelvadnj.html

SELECT TRIM(name) FROM users;
来源：http://hz.svipenyu.cn/gtjrvlmkjv.html

[Q85] 数值取整
来源：http://hz.tianlin.xyz/gtwwukjfvq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.snrcjt.cn/gtxckhhyyu.html

[Q86] 读取 JSON 字段
来源：http://hz.hnxiangtu.top/gtueeoxyem.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shangyingyoupin.top/gtnlutjrzz.html

[Q87] JSON 字段做条件
来源：http://hz.chenjidiqi.icu/gtfdlowfjm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xuetiantiany.cn/gtfujstepw.html

[Q88] 行转列（条件聚合）
来源：http://hz.nwbrower.top/gtuwghnfdp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.svipenyu.cn/gtviiyatdz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.52xcode.cn/gtwqaqsetc.html

[Q89] 判断表是否存在
来源：http://hz.9152youxi.cn/gtdgdfbxya.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nwbrower.top/gtudesgzxh.html

[Q90] 生成序号列
来源：http://hz.snrcjt.cn/gtkzchcofj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.nanxuanxn.top/gtqebccjgu.html

================================================================================
来源：http://hz.cqqwz.cn/gtqrktuapt.html

R. Bash 专题
来源：http://hz.nwbrower.top/gtskyyitum.html

================================================================================
来源：http://hz.shzxlz.cn/gthhktavln.html

[R01] shebang 与严格模式
来源：http://hz.yanxiufei.cn/gtcbfxvasq.html

#!/usr/bin/env bash
来源：http://hz.mhx1999.top/gtycczhmka.html

set -euo pipefail
来源：http://hz.gotoacloud.top/gtrcphvohe.html

[R02] 变量赋值与使用
来源：http://hz.haohaochexian.top/gtlwrqauxb.html

name="Tom"; echo "$name"
来源：http://hz.ywan-chungtsiang.top/gtjzqyxbuy.html

[R03] 只读变量
来源：http://hz.hongshengwenyu.top/gthufalxfo.html

readonly PI=3.14
来源：http://hz.nanxuanxn.top/gtqexmqxaf.html

[R04] 位置参数
来源：http://hz.xuetiantiany.cn/gtmfasgmgu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gaohongyu789.top/gtgocopabl.html

[R05] 参数默认值
来源：http://hz.mhx1999.top/gtrrdoupyr.html

name="${1:-default}"
来源：http://hz.zhengqikj.top/gtovmmesqr.html

[R06] 判断命令是否存在
来源：http://hz.andypj.xyz/gtttyuidhv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj202588.top/gtvbldvwho.html

[R07] if 判断文件
来源：http://hz.havefunace.top/gtbqrctaxp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cashguo.top/gtboagycds.html

[R08] 数值比较
来源：http://hz.hnxiangtu.top/gthijnfxdl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cheryme.top/gtnrwgyime.html

[R09] 字符串比较
来源：http://hz.wangshuangyany.cn/gtqnrvrlat.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jiagoushi.top/gtvtmvhyqm.html

[R10] 正则匹配
来源：http://hz.jyoumei.cn/gtukacfait.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj20258.top/gtkudvoubp.html

[R11] case 多分支
来源：http://hz.wangshuangyany.cn/gtlhvjggea.html

case "$1" in
来源：http://hz.xuanzx.com/gttlhewvyn.html

start) echo "启动" ;;
来源：http://hz.52xcode.cn/gtckadagkk.html

stop)  echo "停止" ;;
来源：http://hz.guannengcc.top/gttkyamvqg.html

*)     echo "未知命令" ;;
来源：http://hz.jlsjyb.cn/gtklumpvnq.html

esac
来源：http://hz.shanyushiyangtech.top/gtzkictmsl.html

[R12] for 遍历文件
来源：http://hz.zhixingplan.top/gtxdqqloyh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.tanke756.top/gtdqvlghxt.html

[R13] for 计数循环
来源：http://hz.jqgufenzy.top/gtlcgsvzvh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hywenlv.cn/gtmorrtwts.html

[R14] C 风格 for
来源：http://hz.daxiang520.top/gtwnllrgrn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.chenjidiqi.icu/gtunzayfod.html

[R15] while 逐行读文件
来源：http://hz.ehwqpu.com/gtrsazcdpb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jqgufenzy.top/gtoyihpcbw.html

[R16] until 等待条件
来源：http://hz.svipenyu.cn/gtezosdndo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gotoacloud.top/gtpjwhswsa.html

[R17] 数组定义与取值
来源：http://hz.zhengqikj.top/gtvlsgkogu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ybcxt.top/gtkjxvgzpt.html

[R18] 遍历数组
来源：http://hz.yangfankeji.com/gttvmerfwk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cucudq.cn/gtarxdvbem.html

[R19] 数组长度
来源：http://hz.gogol.net.cn/gtmmsvayry.html

echo "${#arr[@]}"
来源：http://hz.jlsjyb.cn/gtzkewuwzd.html

[R20] 关联数组（字典）
来源：http://hz.yvedp.cn/gtqkkvyvso.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.pengpengdd.cyou/gtfkrlvmjx.html

[R21] 字符串长度
来源：http://hz.zhixingplan.top/gtehqovsau.html

echo "${#s}"
来源：http://hz.jqgufenzy.top/gtqmtaqlel.html

[R22] 截取子串
来源：http://hz.svipenyu.cn/gtkgleijxb.html

echo "${s:0:5}"
来源：http://hz.zhongyouzk.top/gtzxnuxtva.html

[R23] 字符串替换
来源：http://hz.meibo888.top/gtfamveyzg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.haohaochexian.top/gtdvihxyds.html

[R24] 大小写转换
来源：http://hz.hongshengwenyu.top/gtngsyhucj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yvedp.cn/gtctpbzpsh.html

[R25] 去后缀 / 去前缀
来源：http://hz.ppjwa.cn/gtlwvggswv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinqigufen.top/gtvupelcbs.html

[R26] 命令替换
来源：http://hz.ivvv.top/gtkewksojv.html

now=$(date +%F); echo "$now"
来源：http://hz.aizwys.cn/gtukfzishz.html

[R27] 算术展开
来源：http://hz.gzhubu.top/gtjoqvdhkz.html

echo $((1 + 2 * 3))
来源：http://hz.shanyushiyangtech.top/gttwygcnns.html

[R28] 浮点运算
来源：http://hz.ivvv.top/gtddjjgita.html

echo "scale=2; 10/3" | bc
来源：http://hz.bjfxy.top/gtbjtdcdzq.html

[R29] 定义函数
来源：http://hz.316326.xyz/gtsxablsjx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jiagoushi.top/gtjpppwaji.html

[R30] 函数返回状态码
来源：http://hz.xingfuxueyuan.xyz/gtjlugqtfb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ivvv.top/gtstiilspw.html

[R31] 局部变量
来源：http://hz.jinqigufen.top/gtraqxypie.html

f() { local x=1; echo "$x"; }
来源：http://hz.hongshengwenyu.top/gtumuqoltf.html

[R32] 参数个数校验
来源：http://hz.0kj1m.cn/gtsrhpllbg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.redwolf501.top/gtzrdowjnn.html

[R33] 捕获错误并提示行号
来源：http://hz.yvedp.cn/gttrmqwrkp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yangfankeji.com/gtygxxofnz.html

[R34] 退出时清理
来源：http://hz.jinqigufen.top/gtvmzcicks.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258.top/gtuhsqjxtg.html

[R35] 后台执行并等待
来源：http://hz.cucudq.cn/gtwicjdoyw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yonumen.top/gtghabqqow.html

[R36] 并发执行多个任务
来源：http://hz.xingfuxueyuan.xyz/gtjfwvgybh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhengqikj.top/gtjthebauv.html

[R37] 把输出赋给变量
来源：http://hz.hnxiangtu.top/gtpbvtbxov.html

files=$(ls -1)
来源：http://hz.tanke756.top/gtwkcrxvhi.html

[R38] 管道串联
来源：http://hz.jianghu66.top/gtmmhcjdsn.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj20258.top/gtbivsuwqs.html

[R39] 重定向标准输出与错误
来源：http://hz.zhijiandao.cn/gtynfmkuap.html

cmd > out.log 2>&1
来源：http://hz.jinqigfzy.top/gtvdiqrolg.html

[R40] 追加写日志
来源：http://hz.cucudq.cn/gtgpkoyepd.html

echo "log" >> out.log
来源：http://hz.zhijiandao.cn/gtqraxdake.html

[R41] 丢弃输出
来源：http://hz.jlsjyb.cn/gtnrgjlsbu.html

cmd >/dev/null 2>&1
来源：http://hz.cdnleiting.top/gtanqleyxh.html

[R42] 输入重定向
来源：http://hz.guowangkeji.top/gtxlrpsifz.html

wc -l < a.txt
来源：http://hz.9152youxi.cn/gtsvhjhrtw.html

[R43] 按名字查找文件
来源：http://hz.jianghu66.top/gtjalesmak.html

find . -name "*.log" -type f
来源：http://hz.cheryme.top/gtpxjokyhi.html

[R44] 按修改时间查找
来源：http://hz.yangfankeji.com/gtecyjuxxq.html

find . -mtime -7 -type f
来源：http://hz.daria6918.cn/gtbsztvdqy.html

[R45] 批量删除
来源：http://hz.yj20258888.top/gtjqukmpou.html

find . -name "*.tmp" -delete
来源：http://hz.xinyue.icu/gtjgtugpud.html

[R46] 递归替换文件内容
来源：http://hz.nwbrower.top/gthbldjrgu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ppjwa.cn/gtfokydsjt.html

[R47] sed 单行替换
来源：http://hz.sweek.top/gtbuaphkzs.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.svipenyu.cn/gtyamefzjk.html

[R48] awk 取指定列
来源：http://hz.yj202588.top/gtycpytvnj.html

awk '{print $1, $3}' a.txt
来源：http://hz.xziqi.cn/gtqgmndlba.html

[R49] awk 带条件
来源：http://hz.bjfxy.top/gtvgpswdwu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.pengpengdd.cyou/gtveztiyod.html

[R50] awk 求和
来源：http://hz.cashguo.top/gtxkszdfti.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cucudq.cn/gtkfuyjucf.html

[R51] 排序去重取前几
来源：http://hz.cashguo.top/gtchoeczgf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhijiandao.cn/gtnxkwghbi.html

[R52] 统计行数
来源：http://hz.cqqwz.cn/gttjtxpelk.html

wc -l a.txt
来源：http://hz.mhx1999.top/gthzftsdpx.html

[R53] 查看文件头与实时尾
来源：http://hz.chenlongwang.top/gtqxocihnd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.nanxuanxn.top/gttnvctzkl.html

[R54] 比较两个文件
来源：http://hz.tianlin.xyz/gtwdfacdtw.html

diff a.txt b.txt
来源：http://hz.ehwqpu.com/gtmgtpqjng.html

[R55] 压缩与解压
来源：http://hz.zhixingplan.top/gtileibler.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.snrcjt.cn/gtdyvvwtoz.html

[R56] 远程拷贝
来源：http://hz.sxryk.cn/gtpptrulup.html

scp file user@host:/path/
来源：http://hz.52xcode.cn/gtjqzwtbar.html

[R57] 远程执行命令
来源：http://hz.mhx1999.top/gtyoindzpd.html

ssh user@host 'uptime'
来源：http://hz.yj20258888.top/gtslrckxga.html

[R58] 下载文件
来源：http://hz.xingfuxueyuan.xyz/gtlehscxgg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.birdmap.top/gtcvzlmnso.html

[R59] 发 POST JSON
来源：http://hz.quarkkingdee.top/gtstvkrbeq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.feifeiyinyue.top/gtgccqozoz.html

[R60] 只看 HTTP 状态码
来源：http://hz.birdmap.top/gtraiuqymd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jqgfzy.top/gtohsflpbo.html

[R61] 磁盘占用
来源：http://hz.dianchejie.cn/gtznfucjdk.html

df -h;  du -sh *
来源：http://hz.chenlongwang.top/gtcgnhoqmp.html

[R62] 找最占空间的文件
来源：http://hz.cqqwz.cn/gtbxprnzfb.html

du -ah . | sort -rh | head -10
来源：http://hz.cdnleiting.top/gtiliitsso.html

[R63] 内存与进程
来源：http://hz.sufxvd.cn/gtmuoalqgv.html

free -h;  ps aux | grep nginx
来源：http://hz.kuanghao11.cn/gtwfbzjngr.html

[R64] 结束进程
来源：http://hz.jqgfzy.top/gtywartqpr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cqqwz.cn/gtxdulhkvx.html

[R65] 查看端口占用
来源：http://hz.chenjidiqi.icu/gtxfjqokzy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuanzhike.top/gtdtdvnhge.html

[R66] 定时任务
来源：http://hz.fzhhl.top/gtojsaesck.html

crontab -e;  crontab -l
来源：http://hz.ywan-chungtsiang.top/gtmtzcjtre.html

[R67] 生成随机十六进制串
来源：http://hz.cucudq.cn/gtokqyuecd.html

openssl rand -hex 16
来源：http://hz.yangfankeji.com/gtckldggid.html

[R68] 计算文件校验值
来源：http://hz.hnqzz.top/gtzaxgfrre.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guowangkeji.top/gthyelxtka.html

[R69] 生成随机密码
来源：http://hz.nanxuanxn.top/gtjkkydgzs.html

head -c 16 /dev/urandom | base64
来源：http://hz.52xcode.cn/gtmtyskryc.html

[R70] 时间戳与互转
来源：http://hz.wangshuangyany.cn/gtrwayvcml.html

date +%s;  date -d @1700000000
来源：http://hz.jqgufenzy.top/gttdvpqqvn.html

[R71] 日期格式化
来源：http://hz.cashguo.top/gtfzcwtbyp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.guowangkeji.top/gtalatruid.html

[R72] 等待端口就绪
来源：http://hz.jyoumei.cn/gtwtictvzz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yueranfly.top/gthkxrmqlp.html

[R73] 分割大日志
来源：http://hz.c1oappe.top/gtcywngjdm.html

split -l 1000 big.log part_
来源：http://hz.gaohongyu789.top/gtpkhcobkv.html

[R74] 批量重命名
来源：http://hz.zhoulong.xyz/gtlkllwfqy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.pengpengdd.cyou/gtfnacqfff.html

[R75] 导出环境变量
来源：http://hz.jinyuanbaomall.cn/gtbndtrbme.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sysykeji.top/gtaruxgdgm.html

[R76] 使用临时文件
来源：http://hz.zhengqikj.top/gtjliqfjet.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.snrcjt.cn/gtnxwdszaw.html

[R77] 读取用户输入
来源：http://hz.hnxiangtu.top/gtscbjgvmu.html

read -rp "请输入: " ans
来源：http://hz.tianlin.xyz/gtaqpndpie.html

[R78] 交互式菜单
来源：http://hz.aizwys.cn/gtelbqchbn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.c1oappe.top/gtikpmizir.html

[R79] 解析命令行选项
来源：http://hz.guowangkeji.top/gtjtvtqwgc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xinyue.icu/gtyjlsxjpq.html

[R80] 查看脚本执行耗时
来源：http://hz.sufxvd.cn/gtacghnfdy.html

time ./run.sh
来源：http://hz.hnqzz.top/gtdcusfayp.html

================================================================================
来源：http://hz.sufxvd.cn/gtmcafelwy.html

S. C / C++ 专题
来源：http://hz.9152youxi.cn/gtotrnfnma.html

================================================================================
来源：http://hz.ivvv.top/gtggmfabke.html

[S01] C：Hello World
来源：http://hz.nanxinkj.top/gthrllgcli.html

#include <stdio.h>
来源：http://hz.zhixingplan.top/gtluqfunob.html


<!-- 参考信息 -->