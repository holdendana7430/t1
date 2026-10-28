代发 wailian999

[Q33] 多列分组
来源：http://hz.hysaishi.cn/gtsorzxgat.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.52xcode.cn/gtjhxbnema.html

[Q34] 每组取第一条
来源：http://hz.hfpthk.cn/gtrosebxxv.html

SELECT * FROM (
来源：http://hz.yongpay.top/gtbittorls.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yongpay.top/gtgxlalqos.html

) t WHERE rn = 1;
来源：http://hz.jianghu66.top/gtooqfgctk.html

[Q35] 内连接
来源：http://hz.smart0.xyz/gtbixbsvbi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yonumen.top/gthccmttzx.html

[Q36] 左连接
来源：http://hz.shzxlz.cn/gtkujipzpg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ybcxt.top/gtbcuwlfpv.html

[Q37] 右连接
来源：http://hz.jiagoushi.top/gtltlphqnx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenzaomai.com/gtyejgzzrm.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sysykeji.top/gtrntkcwnj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.52xcode.cn/gtefmwlywj.html

[Q39] 自连接（查上下级）
来源：http://hz.yueranfly.top/gtmhpqwdsj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xingfuxueyuan.xyz/gtrzykiiyt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xziqi.cn/gtcxbixurr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhongyouzk.top/gtjrstfjkt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.mhx1999.top/gthvphfmdn.html

[Q41] 多表连接
来源：http://hz.sweek.top/gtksxmriqr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shzxlz.cn/gtdupewnvf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.316326.xyz/gtghwpblcw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shangyingyoupin.top/gtsrngpglw.html

[Q42] 连接条件附加过滤
来源：http://hz.sxryk.cn/gtnvllwayo.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yuanzhike.top/gtxrpghuip.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.haohaochexian.top/gtlejuiroy.html

[Q43] 标量子查询
来源：http://hz.mhx1999.top/gtszsafndk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jqgufenzy.top/gtqwusphbd.html

[Q44] IN 子查询
来源：http://hz.vqdsnc.cn/gttkfqtlhh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.snrcjt.cn/gthtvnffwa.html

[Q45] EXISTS 判断存在
来源：http://hz.yj202588.top/gtwtyzajzh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cucudq.cn/gtfyrpwcwc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nanxuanxn.top/gtilphxkja.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jyoumei.cn/gtuwmvpwtr.html

[Q47] 与平均值比较
来源：http://hz.smart0.xyz/gtnjpzpdwx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.iojbl.cn/gtxgokmtzf.html

[Q48] CTE 公用表表达式
来源：http://hz.ppjwa.cn/gtvlgvsptg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.fzhhl.top/gtbafjwokz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.snrcjt.cn/gtygezigau.html

[Q49] 更新单行
来源：http://hz.aibaodan.cn/gtdjbeujqp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cheryme.top/gtoarfyznp.html

[Q50] 批量更新
来源：http://hz.zhixingplan.top/gtqsaonsbc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhixingplan.top/gtgbkqcjsf.html

[Q51] 用子查询更新
来源：http://hz.wangdashe.top/gtnpgjrara.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.havefunace.top/gtkvnpvelw.html

[Q52] 删除指定行
来源：http://hz.xinyue.icu/gtdjamllgn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj20258.top/gtqggrgttv.html

[Q53] 按条件删除
来源：http://hz.smart0.xyz/gtomqxynov.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhijiandao.cn/gtdumbgovr.html

[Q54] 清空表
来源：http://hz.yonumen.top/gtiuzipxlm.html

TRUNCATE TABLE logs;
来源：http://hz.ydzc1.top/gtkeniarjs.html

[Q55] 排名（并列占位）
来源：http://hz.jlsjyb.cn/gtowhftplv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.sxryk.cn/gtilhrivba.html

[Q56] 密集排名（并列不占位）
来源：http://hz.kuanghao11.cn/gtvcfvprwi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cucudq.cn/gtphnumwsz.html

[Q57] 行号
来源：http://hz.zhoulong.xyz/gtcwmtcgnc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.nanxinkj.top/gtbbfokrlf.html

[Q58] 累计求和
来源：http://hz.hongshengwenyu.top/gtcgfkiwjt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ivvv.top/gtidktvwsk.html

[Q59] 分组内累计
来源：http://hz.jqgfzy.top/gtomdozksf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangtech.top/gtswnxkrjl.html

[Q60] 取上一行 / 下一行
来源：http://hz.hfpthk.cn/gtfioqlwye.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jqgufenzy.top/gtxoytbqha.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.9152youxi.cn/gtqwzenyel.html

[Q61] 移动平均
来源：http://hz.daria6918.cn/gtsmjcqiys.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yonumen.top/gtzykgfwkb.html

[Q62] 分组占比
来源：http://hz.smart0.xyz/gtcfsvepwx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtavhvzkcp.html

[Q63] 开启事务
来源：http://hz.jqgfzy.top/gtkwhtazdq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ydzc1.top/gtfxmijpas.html

[Q64] 提交事务
来源：http://hz.jinqigfzy.top/gtnohmisxo.html

COMMIT;
来源：http://hz.ybcxt.top/gtayyvaruq.html

[Q65] 回滚事务
来源：http://hz.hysaishi.cn/gtvlxljxnd.html

ROLLBACK;
来源：http://hz.zycfv.cn/gtbhzfqyzr.html

[Q66] 行锁查询
来源：http://hz.jlsjyb.cn/gttuimnkfj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ywan-chungtsiang.top/gtclvyrtoz.html

[Q67] 设置隔离级别
来源：http://hz.ehwqpu.com/gtdwfxjxfi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.dashuyun.cn/gtfsyvveya.html

[Q68] 保存点
来源：http://hz.daria6918.cn/gthvvbyrtm.html

SAVEPOINT sp1;
来源：http://hz.jinqigfzy.top/gtfmqzyrli.html

ROLLBACK TO sp1;
来源：http://hz.zhijiandao.cn/gtywmnmcbr.html

[Q69] 查看执行计划
来源：http://hz.jlsjyb.cn/gtoztworzs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nanxinkj.top/gtlrmtgmtr.html

[Q70] 更新统计信息
来源：http://hz.yangfankeji.com/gttkkgtrjy.html

ANALYZE TABLE users;
来源：http://hz.xinyue.icu/gtvxdqudnd.html

[Q71] 查看建表语句
来源：http://hz.xuetiantiany.cn/gtxrdnglnx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ivvv.top/gtyapsstou.html

[Q72] 查看索引
来源：http://hz.yangfankeji.com/gtrforwael.html

SHOW INDEX FROM users;
来源：http://hz.zhiwuduotai.top/gtgaezvxzs.html

[Q73] 查看表状态
来源：http://hz.chenzaomai.com/gtzpjlsqwr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yongpay.top/gtfbmhgcjk.html

[Q74] 强制使用索引
来源：http://hz.yuanzhike.top/gtljqhyhqn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.wangdashe.top/gtrljorksi.html

[Q75] 日期格式化
来源：http://hz.xingfuxueyuan.xyz/gtezesafsh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.havefunace.top/gtkjpbzkcl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinqigfzy.top/gtpuraownw.html

[Q76] 按天统计
来源：http://hz.andypj.xyz/gthehkfwyd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zycfv.cn/gtnaqwqupk.html

[Q77] 时间加减
来源：http://hz.sxryk.cn/gtpdhksdvs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhijiandao.cn/gtesozpupa.html

[Q78] 当前时间
来源：http://hz.shanyushiyangkeji.top/gtwbcaglet.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.0kj1m.cn/gtebftzsvx.html

[Q79] 字符串拼接
来源：http://hz.bjfxy.top/gtwevhkeqt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ehwqpu.com/gtwvagvaae.html

[Q80] 字符串截取
来源：http://hz.zhijiandao.cn/gtlisqbeuj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xinyue.icu/gttatidqkg.html

[Q81] 字符串替换
来源：http://hz.gzhubu.top/gtkciepveu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tian-w.cn/gtxvtutpgy.html

[Q82] 字符长度与字节长度
来源：http://hz.hammf.cn/gtlqhloaki.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.bjfxy.top/gtcceoryzg.html

[Q83] 大小写转换
来源：http://hz.svipenyu.cn/gtflehwiou.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.aizwys.cn/gtvyayzzbk.html

[Q84] 去除首尾空格
来源：http://hz.yj202588.top/gtnqiuwaqw.html

SELECT TRIM(name) FROM users;
来源：http://hz.ydjk.org.cn/gtbafdyrth.html

[Q85] 数值取整
来源：http://hz.jinyuanbaomall.cn/gtddfzswhb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ydzc1.top/gtpmuskzpk.html

[Q86] 读取 JSON 字段
来源：http://hz.andypj.xyz/gtnqrcacnf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.havefunace.top/gtbiouhjcm.html

[Q87] JSON 字段做条件
来源：http://hz.ydjk.org.cn/gteuwmbvzk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zdqjudy.top/gttvkgvnyi.html

[Q88] 行转列（条件聚合）
来源：http://hz.gotoacloud.top/gtowriwnrq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sweek.top/gtqgurextb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yangfankeji.com/gtzfdhuwma.html

[Q89] 判断表是否存在
来源：http://hz.0kj1m.cn/gtdteuczwa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tianlin.xyz/gtsuzsgimm.html

[Q90] 生成序号列
来源：http://hz.chenjidiqi.icu/gthonjgdpd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yj202588.top/gtzwewxqvv.html

================================================================================
来源：http://hz.tanke756.top/gtjevoqnwe.html

R. Bash 专题
来源：http://hz.hysaishi.cn/gtbzcavyaf.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtxdkzfrbo.html

[R01] shebang 与严格模式
来源：http://hz.jianghu66.top/gtcgdvfagx.html

#!/usr/bin/env bash
来源：http://hz.wangdashe.top/gtvzkpqcjx.html

set -euo pipefail
来源：http://hz.xylfe.cn/gtgbqckgla.html

[R02] 变量赋值与使用
来源：http://hz.tianlin.xyz/gtazfbwfhu.html

name="Tom"; echo "$name"
来源：http://hz.zhaomingkeji.xyz/gtesuysido.html

[R03] 只读变量
来源：http://hz.wangshuangyany.cn/gtalkaltfp.html

readonly PI=3.14
来源：http://hz.zycfv.cn/gtmamlsnny.html

[R04] 位置参数
来源：http://hz.jinyuanbaomall.cn/gtjncjassn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.birdmap.top/gtllbrfswn.html

[R05] 参数默认值
来源：http://hz.sweek.top/gtyvkryvvd.html

name="${1:-default}"
来源：http://hz.daxiang520.top/gtrdsczcry.html

[R06] 判断命令是否存在
来源：http://hz.jinqigfzy.top/gtcuyzrxav.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zycfv.cn/gteprgircv.html

[R07] if 判断文件
来源：http://hz.daria6918.cn/gtlcshwfcv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sweek.top/gtxvuhvilp.html

[R08] 数值比较
来源：http://hz.shanyushiyangkeji.top/gtxgozqbqt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hongshengwenyu.top/gtnhzweaag.html

[R09] 字符串比较
来源：http://hz.gotoacloud.top/gtvtoebzby.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.nanxuanxn.top/gtratpkpxn.html

[R10] 正则匹配
来源：http://hz.gaohongyu789.top/gtjwoelhcx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.vqdsnc.cn/gtnaispjia.html

[R11] case 多分支
来源：http://hz.pycfn.com/gtlmciguiv.html

case "$1" in
来源：http://hz.gogol.net.cn/gtdwohkkmf.html

start) echo "启动" ;;
来源：http://hz.c1oappe.top/gtxjrkrhrj.html

stop)  echo "停止" ;;
来源：http://hz.nanxinkj.top/gturxhkeze.html

*)     echo "未知命令" ;;
来源：http://hz.hnqzz.top/gtefcxhdfs.html

esac
来源：http://hz.yvedp.cn/gtdgkspfpe.html

[R12] for 遍历文件
来源：http://hz.0kj1m.cn/gtfujcdwgc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yvedp.cn/gtacahhjid.html

[R13] for 计数循环
来源：http://hz.ybcxt.top/gtgtwutrum.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.wangshuangyany.cn/gthjvkvmxr.html

[R14] C 风格 for
来源：http://hz.316326.xyz/gtvjhpljrb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nwbrower.top/gtnbrenovp.html

[R15] while 逐行读文件
来源：http://hz.yj202588.top/gtlrngfwrs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinyuanbaomall.cn/gtdetuovmi.html

[R16] until 等待条件
来源：http://hz.jiagoushi.top/gttvfgszuw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yanxiufei.cn/gtuqhojlaf.html

[R17] 数组定义与取值
来源：http://hz.hnqzz.top/gtisobrgya.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cheryme.top/gtpjqmsgjb.html

[R18] 遍历数组
来源：http://hz.dashuyun.cn/gtdykjfwub.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jianghu66.top/gtjkzmvsgh.html

[R19] 数组长度
来源：http://hz.ehwqpu.com/gtqdbxuwfb.html

echo "${#arr[@]}"
来源：http://hz.cqqwz.cn/gtgguvtxqs.html

[R20] 关联数组（字典）
来源：http://hz.redwolf501.top/gtvdfmmymc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jyoumei.cn/gtqlnrcjvp.html

[R21] 字符串长度
来源：http://hz.nanxinkj.top/gtctbelpca.html

echo "${#s}"
来源：http://hz.vqdsnc.cn/gtecxlgxnf.html

[R22] 截取子串
来源：http://hz.jqgufenzy.top/gtbgkaabdw.html

echo "${s:0:5}"
来源：http://hz.jyoumei.cn/gtsvekkmko.html

[R23] 字符串替换
来源：http://hz.sufxvd.cn/gtytdhkpck.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgufenzy.top/gttmubzghc.html

[R24] 大小写转换
来源：http://hz.shuidangran.top/gtymxtqcud.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.snrcjt.cn/gtoswpdxba.html

[R25] 去后缀 / 去前缀
来源：http://hz.ppjwa.cn/gtuwglpftp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yj20258.top/gtvuryevxp.html

[R26] 命令替换
来源：http://hz.zhoulong.xyz/gtmqfonltc.html

now=$(date +%F); echo "$now"
来源：http://hz.zhongyouzk.top/gtgqrmvjmy.html

[R27] 算术展开
来源：http://hz.hnqzz.top/gtwfinrlwv.html

echo $((1 + 2 * 3))
来源：http://hz.yvedp.cn/gtwozuxneu.html

[R28] 浮点运算
来源：http://hz.cqqwz.cn/gtnguhyyhe.html

echo "scale=2; 10/3" | bc
来源：http://hz.cheryme.top/gtheenpgjv.html

[R29] 定义函数
来源：http://hz.pengpengdd.cyou/gtuvdpbzxl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hongshengwenyu.top/gtlfepwzat.html

[R30] 函数返回状态码
来源：http://hz.wangshuangyany.cn/gtggherxsp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pengpengdd.cyou/gtnqbuqrcw.html

[R31] 局部变量
来源：http://hz.fzhhl.top/gtxtkxgcss.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhaomingkeji.xyz/gtedvdffre.html

[R32] 参数个数校验
来源：http://hz.jqgufenzy.top/gtuuftnibq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.guowangkeji.top/gtvtykjtoa.html

[R33] 捕获错误并提示行号
来源：http://hz.jqgufenzy.top/gtezepszab.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.fengsongda.top/gtciiwoxpc.html

[R34] 退出时清理
来源：http://hz.ppjwa.cn/gtvvselymj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gtotoikikw.html

[R35] 后台执行并等待
来源：http://hz.andypj.xyz/gtozbzwstu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shanyushiyangtech.top/gtloqkdurd.html

[R36] 并发执行多个任务
来源：http://hz.haohaochexian.top/gtmokruhvc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shanyushiyangtech.top/gtroawkudi.html

[R37] 把输出赋给变量
来源：http://hz.nanxinkj.top/gtmthfoucb.html

files=$(ls -1)
来源：http://hz.kuanghao11.cn/gtfympplzo.html

[R38] 管道串联
来源：http://hz.redwolf501.top/gtfgfrwzxt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xingfuxueyuan.xyz/gtzzfxuirr.html

[R39] 重定向标准输出与错误
来源：http://hz.shanyushiyangkeji.top/gtmawtnoyn.html

cmd > out.log 2>&1
来源：http://hz.xuanzx.com/gtrkqdzwkw.html

[R40] 追加写日志
来源：http://hz.meibo888.top/gtdugvqwes.html

echo "log" >> out.log
来源：http://hz.nanxinkj.top/gtoilwfpau.html

[R41] 丢弃输出
来源：http://hz.pycfn.com/gtmdzadtzg.html

cmd >/dev/null 2>&1
来源：http://hz.dashuyun.cn/gtyrheydhz.html

[R42] 输入重定向
来源：http://hz.snrcjt.cn/gtwfqrtlje.html

wc -l < a.txt
来源：http://hz.hnxiangtu.top/gtksulyecw.html

[R43] 按名字查找文件
来源：http://hz.yuxming.cn/gtexunnmvr.html

find . -name "*.log" -type f
来源：http://hz.jianghu66.top/gtozyasgmt.html

[R44] 按修改时间查找
来源：http://hz.iojbl.cn/gtscqejnam.html

find . -mtime -7 -type f
来源：http://hz.fzhhl.top/gttfkhcont.html

[R45] 批量删除
来源：http://hz.shzxlz.cn/gtgnpplsoy.html

find . -name "*.tmp" -delete
来源：http://hz.shanyushiyangtech.top/gteliscaja.html

[R46] 递归替换文件内容
来源：http://hz.zhengqikj.top/gtmvltmwmo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.chenzaomai.com/gtbnpqwxrk.html

[R47] sed 单行替换
来源：http://hz.feifeiyinyue.top/gtjmdalqla.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ehwqpu.com/gtcgecnagl.html

[R48] awk 取指定列
来源：http://hz.shzxlz.cn/gtvwqnxlqu.html

awk '{print $1, $3}' a.txt
来源：http://hz.aibaodan.cn/gtxgfqdrrw.html

[R49] awk 带条件
来源：http://hz.tanke756.top/gtiptldjgf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yonumen.top/gtfwzgvsgi.html

[R50] awk 求和
来源：http://hz.shzxlz.cn/gtvukvrcem.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.tanke756.top/gtcowqieob.html

[R51] 排序去重取前几
来源：http://hz.sxryk.cn/gtaixtsguq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.kuanghao11.cn/gtkamnilcp.html

[R52] 统计行数
来源：http://hz.tanke756.top/gtacxhihiv.html

wc -l a.txt
来源：http://hz.yonumen.top/gtvbfcvjvj.html

[R53] 查看文件头与实时尾
来源：http://hz.jqgufenzy.top/gtlibtgvpu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hnqzz.top/gtdtxmshya.html

[R54] 比较两个文件
来源：http://hz.gogol.net.cn/gtythkqtit.html

diff a.txt b.txt
来源：http://hz.dashuyun.cn/gteugdjzkj.html

[R55] 压缩与解压
来源：http://hz.xziqi.cn/gtfnfdlerz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zdqjudy.top/gtqxxsllrp.html

[R56] 远程拷贝
来源：http://hz.jqgufenzy.top/gtnnbsvlnv.html

scp file user@host:/path/
来源：http://hz.ehwqpu.com/gtydypvxpx.html

[R57] 远程执行命令
来源：http://hz.tianlin.xyz/gtiyjdqerd.html

ssh user@host 'uptime'
来源：http://hz.guowangkeji.top/gtzkrsawrw.html

[R58] 下载文件
来源：http://hz.yuxming.cn/gtatoyhjpf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jianghu66.top/gtqmxzascb.html

[R59] 发 POST JSON
来源：http://hz.cheryme.top/gtjuipkbcf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.vqdsnc.cn/gthqrvlgdj.html

[R60] 只看 HTTP 状态码
来源：http://hz.cqqwz.cn/gtwbephtep.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhaomingkeji.xyz/gtelmdvibn.html

[R61] 磁盘占用
来源：http://hz.xingfuxueyuan.xyz/gtdqhfmztv.html

df -h;  du -sh *
来源：http://hz.gaohongyu789.top/gtwamqwxcv.html

[R62] 找最占空间的文件
来源：http://hz.hywenlv.cn/gtsxklzqjo.html

du -ah . | sort -rh | head -10
来源：http://hz.0kj1m.cn/gtfvdbmnjh.html

[R63] 内存与进程
来源：http://hz.nanxuanxn.top/gtknuhcsaf.html

free -h;  ps aux | grep nginx
来源：http://hz.c1oappe.top/gtitkpqbcb.html

[R64] 结束进程
来源：http://hz.ydjk.org.cn/gtunubpfwk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yangfankeji.com/gtvllnhupy.html

[R65] 查看端口占用
来源：http://hz.cqqwz.cn/gtsgvisxty.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jqgufenzy.top/gtyllrxuka.html

[R66] 定时任务
来源：http://hz.iojbl.cn/gteuwiekbn.html

crontab -e;  crontab -l
来源：http://hz.shuidangran.top/gtmjnevesn.html

[R67] 生成随机十六进制串
来源：http://hz.guannengcc.top/gtudenokyu.html

openssl rand -hex 16
来源：http://hz.hysaishi.cn/gtnmdxyxjt.html

[R68] 计算文件校验值
来源：http://hz.0kj1m.cn/gtrfjactrr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guannengcc.top/gtxquklbwu.html

[R69] 生成随机密码
来源：http://hz.tian-w.cn/gtbumaijwt.html

head -c 16 /dev/urandom | base64
来源：http://hz.nanxuanxn.top/gtfdasjmdt.html

[R70] 时间戳与互转
来源：http://hz.dianchejie.cn/gttkzxxgmr.html

date +%s;  date -d @1700000000
来源：http://hz.316326.xyz/gtcddztbrk.html

[R71] 日期格式化
来源：http://hz.gotoacloud.top/gtkvpdqkzg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.bjfxy.top/gtvjnjbffu.html

[R72] 等待端口就绪
来源：http://hz.ywan-chungtsiang.top/gtkitnmayi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hfpthk.cn/gtxzjugjpc.html

[R73] 分割大日志
来源：http://hz.316326.xyz/gtzonhvtnl.html

split -l 1000 big.log part_
来源：http://hz.xingfuxueyuan.xyz/gtaidjrzvo.html

[R74] 批量重命名
来源：http://hz.zhoulong.xyz/gtpnsozlxy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.dashuyun.cn/gtwyhaleef.html

[R75] 导出环境变量
来源：http://hz.shuidangran.top/gtfbdjiexs.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.daria6918.cn/gtinjzyqmd.html

[R76] 使用临时文件
来源：http://hz.yonumen.top/gtucortafj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.aibaodan.cn/gtbuktaeiv.html

[R77] 读取用户输入
来源：http://hz.ywan-chungtsiang.top/gtmxllqhiq.html

read -rp "请输入: " ans
来源：http://hz.cheryme.top/gtupshljga.html

[R78] 交互式菜单
来源：http://hz.iojbl.cn/gtmteglrhs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xinyue.icu/gtelfhwsit.html

[R79] 解析命令行选项
来源：http://hz.shuidangran.top/gtkrotshco.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sysykeji.top/gtadoxliro.html

[R80] 查看脚本执行耗时
来源：http://hz.jinqigfzy.top/gtutiujkvv.html

time ./run.sh
来源：http://hz.nanxinkj.top/gtdkmemesa.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtmaotcsjt.html

S. C / C++ 专题
来源：http://hz.tianlin.xyz/gtubezxsam.html

================================================================================
来源：http://hz.ehwqpu.com/gtiguayeda.html

[S01] C：Hello World
来源：http://hz.yj202588.top/gtkqqzrjvu.html

#include <stdio.h>
来源：http://hz.sxryk.cn/gtkblxlqvo.html


<!-- 参考信息 -->