代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://hz.guannengcc.top/gtziopabaa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xinyue.icu/gtdviiskfx.html

[Q39] 自连接（查上下级）
来源：http://hz.chenlongwang.top/gttnbpkyzg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.svipenyu.cn/gtcsaghtrf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ydzc1.top/gttwchnrdx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.daria6918.cn/gtqhemytgv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xuanzx.com/gtpmfggsfi.html

[Q41] 多表连接
来源：http://hz.sweek.top/gtkmwrkuqq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tianlin.xyz/gtbzrogjhk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yongpay.top/gtxyddulfw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinqigufen.top/gtnerpikqv.html

[Q42] 连接条件附加过滤
来源：http://hz.guannengcc.top/gtmwsicrzh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xuanzx.com/gtywlzxlzq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jianghu66.top/gtfdmtezcn.html

[Q43] 标量子查询
来源：http://hz.mhx1999.top/gtwjynpiuz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhoulong.xyz/gtfdvfuadd.html

[Q44] IN 子查询
来源：http://hz.snrcjt.cn/gtdpklpntz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sweek.top/gtupbqmxdx.html

[Q45] EXISTS 判断存在
来源：http://hz.mhx1999.top/gtawhribcs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jiagoushi.top/gtbjgbfjia.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gaohongyu789.top/gtjyjdlhui.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yonumen.top/gtatsognlq.html

[Q47] 与平均值比较
来源：http://hz.smart0.xyz/gtmewmgubr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yueranfly.top/gtdgffbhzx.html

[Q48] CTE 公用表表达式
来源：http://hz.zhaomingkeji.xyz/gthmlvjatv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xuanzx.com/gtjpfwavvi.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj20258.top/gtcteyyjbr.html

[Q49] 更新单行
来源：http://hz.c1oappe.top/gtvuooevbg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.snrcjt.cn/gtwukvziod.html

[Q50] 批量更新
来源：http://hz.zhijiandao.cn/gtuykxtcmg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.daria6918.cn/gtctqtfynz.html

[Q51] 用子查询更新
来源：http://hz.chenjidiqi.icu/gtgzevfbry.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yonumen.top/gtvyhtingp.html

[Q52] 删除指定行
来源：http://hz.redwolf501.top/gtirbjumzr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ywan-chungtsiang.top/gtjkqjzfsc.html

[Q53] 按条件删除
来源：http://hz.quarkkingdee.top/gtogzongbr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.svipenyu.cn/gtjvbtpydk.html

[Q54] 清空表
来源：http://hz.xingfuxueyuan.xyz/gtbgzeqohh.html

TRUNCATE TABLE logs;
来源：http://hz.nwbrower.top/gtmimddhbf.html

[Q55] 排名（并列占位）
来源：http://hz.sufxvd.cn/gtrufycfgu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shanyushiyangtech.top/gtwnylqqnd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.bjfxy.top/gtzmfaftby.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.vqdsnc.cn/gthxomqylo.html

[Q57] 行号
来源：http://hz.hysaishi.cn/gtauzadwwu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yj20258888.top/gtfjenvjhd.html

[Q58] 累计求和
来源：http://hz.yj202588.top/gtkxnbtbvf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zdqjudy.top/gtzeistkck.html

[Q59] 分组内累计
来源：http://hz.cheryme.top/gtuynlxyhy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hnqzz.top/gtyoxwsffl.html

[Q60] 取上一行 / 下一行
来源：http://hz.pycfn.com/gtqbmppqnr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ppjwa.cn/gttlyiyfzp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhoulong.xyz/gtdqiqckew.html

[Q61] 移动平均
来源：http://hz.jinghuilouyu.cn/gtvosswwaf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.iojbl.cn/gtvvnljwab.html

[Q62] 分组占比
来源：http://hz.guowangkeji.top/gtnyygpvua.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.havefunace.top/gtyevnkaoo.html

[Q63] 开启事务
来源：http://hz.vqdsnc.cn/gtgxsllimw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jqgfzy.top/gtjnanskcg.html

[Q64] 提交事务
来源：http://hz.ivvv.top/gtnmkxfuax.html

COMMIT;
来源：http://hz.pengpengdd.cyou/gtrlhjbotd.html

[Q65] 回滚事务
来源：http://hz.ehwqpu.com/gtuwimbigb.html

ROLLBACK;
来源：http://hz.cashguo.top/gtiitmatkx.html

[Q66] 行锁查询
来源：http://hz.jiagoushi.top/gtuncfeqou.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gzhubu.top/gtfwiphhwk.html

[Q67] 设置隔离级别
来源：http://hz.ivvv.top/gtmhryaxyr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shuidangran.top/gtcrhzxoqi.html

[Q68] 保存点
来源：http://hz.bjfxy.top/gtxoyrhhcs.html

SAVEPOINT sp1;
来源：http://hz.gogol.net.cn/gtaxykqytv.html

ROLLBACK TO sp1;
来源：http://hz.316326.xyz/gtostvuilh.html

[Q69] 查看执行计划
来源：http://hz.wangdashe.top/gtbefrdfhu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cdnleiting.top/gtcfsqsbsg.html

[Q70] 更新统计信息
来源：http://hz.jinqigfzy.top/gtkjjwtegy.html

ANALYZE TABLE users;
来源：http://hz.sufxvd.cn/gthnwjweww.html

[Q71] 查看建表语句
来源：http://hz.sweek.top/gtikptsigf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xziqi.cn/gtwhgzmyte.html

[Q72] 查看索引
来源：http://hz.yj202588.top/gtveyecjba.html

SHOW INDEX FROM users;
来源：http://hz.hnqzz.top/gthpkpwvrs.html

[Q73] 查看表状态
来源：http://hz.aibaodan.cn/gtmxsqnwys.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shanyushiyangtech.top/gtunktbvae.html

[Q74] 强制使用索引
来源：http://hz.fzhhl.top/gtlvfoodkl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jqgufenzy.top/gtmbkowugp.html

[Q75] 日期格式化
来源：http://hz.zhongyouzk.top/gtmiovpkes.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtejojpkvk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nwbrower.top/gtnghflbwx.html

[Q76] 按天统计
来源：http://hz.chenjidiqi.icu/gtfvrrkqwh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yj202588.top/gtbyeazsit.html

[Q77] 时间加减
来源：http://hz.zhongyouzk.top/gticasltxq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cheryme.top/gthnwzezxz.html

[Q78] 当前时间
来源：http://hz.chenjidiqi.icu/gtcxoemflm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hnqzz.top/gtqtqvukij.html

[Q79] 字符串拼接
来源：http://hz.birdmap.top/gtwyjdwoxx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.guowangkeji.top/gtjvbaqwjq.html

[Q80] 字符串截取
来源：http://hz.haohaochexian.top/gtlntiqvha.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yuanzhike.top/gtpwkecjvx.html

[Q81] 字符串替换
来源：http://hz.yueranfly.top/gtrktcrvhe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhongyouzk.top/gtquzsklpo.html

[Q82] 字符长度与字节长度
来源：http://hz.wangshuangyany.cn/gtqcmhcigf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.0kj1m.cn/gtcqjojpvm.html

[Q83] 大小写转换
来源：http://hz.chenzaomai.com/gtbemiuphb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nanxinkj.top/gtyuujnvvy.html

[Q84] 去除首尾空格
来源：http://hz.aizwys.cn/gtiqwkqdaf.html

SELECT TRIM(name) FROM users;
来源：http://hz.yj202588.top/gtlvdziwoq.html

[Q85] 数值取整
来源：http://hz.hysaishi.cn/gtysrhxvsa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yj20258.top/gtoaifgbqs.html

[Q86] 读取 JSON 字段
来源：http://hz.ybcxt.top/gtjtvonnsn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yonumen.top/gtumshyojz.html

[Q87] JSON 字段做条件
来源：http://hz.hnqzz.top/gttcpjbzey.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ehwqpu.com/gthuljxgzv.html

[Q88] 行转列（条件聚合）
来源：http://hz.sufxvd.cn/gtzmcvikyw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cucudq.cn/gtnvqxbfva.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yangfankeji.com/gtswsujtmp.html

[Q89] 判断表是否存在
来源：http://hz.sxryk.cn/gtcunzyxxc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinqigfzy.top/gtpnyyhzrr.html

[Q90] 生成序号列
来源：http://hz.chenlongwang.top/gtctomhzrq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.svipenyu.cn/gtzmubqapz.html

================================================================================
来源：http://hz.meibo888.top/gtbhbwodwe.html

R. Bash 专题
来源：http://hz.daria6918.cn/gtzawqxhuy.html

================================================================================
来源：http://hz.jlsjyb.cn/gtpdxldilc.html

[R01] shebang 与严格模式
来源：http://hz.sweek.top/gtlxymesbo.html

#!/usr/bin/env bash
来源：http://hz.ywan-chungtsiang.top/gtmftmmwuf.html

set -euo pipefail
来源：http://hz.chenzaomai.com/gthwedzolz.html

[R02] 变量赋值与使用
来源：http://hz.pengpengdd.cyou/gtmchhvizy.html

name="Tom"; echo "$name"
来源：http://hz.aizwys.cn/gtyjlawjxs.html

[R03] 只读变量
来源：http://hz.bjfxy.top/gtoinojgdv.html

readonly PI=3.14
来源：http://hz.gogol.net.cn/gtvuqonkkk.html

[R04] 位置参数
来源：http://hz.mhx1999.top/gtuibuwita.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.pycfn.com/gtmtohpefb.html

[R05] 参数默认值
来源：http://hz.ywan-chungtsiang.top/gtqspizrtf.html

name="${1:-default}"
来源：http://hz.zhaomingkeji.xyz/gttwscwxkj.html

[R06] 判断命令是否存在
来源：http://hz.zhijiandao.cn/gtpwotpuuk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.daria6918.cn/gtczfbcraw.html

[R07] if 判断文件
来源：http://hz.xuetiantiany.cn/gtzwlauwie.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hysaishi.cn/gtuostzjsn.html

[R08] 数值比较
来源：http://hz.cucudq.cn/gtlcsqzsow.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.daxiang520.top/gtdhwxzopq.html

[R09] 字符串比较
来源：http://hz.jiagoushi.top/gtugbdynzc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydjk.org.cn/gtgqorlflx.html

[R10] 正则匹配
来源：http://hz.tianlin.xyz/gtbnuymwbo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gzhubu.top/gtrfhlzzza.html

[R11] case 多分支
来源：http://hz.jianghu66.top/gtibwhzbkh.html

case "$1" in
来源：http://hz.cqqwz.cn/gtmwbngjga.html

start) echo "启动" ;;
来源：http://hz.haohaochexian.top/gtprrcgdph.html

stop)  echo "停止" ;;
来源：http://hz.zhengqikj.top/gtsvexignm.html

*)     echo "未知命令" ;;
来源：http://hz.yanxiufei.cn/gtqgtgzjjn.html

esac
来源：http://hz.xziqi.cn/gtlqcsznyz.html

[R12] for 遍历文件
来源：http://hz.hnqzz.top/gtgeqqwveh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.havefunace.top/gtgpjnnhou.html

[R13] for 计数循环
来源：http://hz.zhiwuduotai.top/gtqdbjkffq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hysaishi.cn/gtuodnyoer.html

[R14] C 风格 for
来源：http://hz.daria6918.cn/gtbwyzpeon.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.bjfxy.top/gtmudljkxw.html

[R15] while 逐行读文件
来源：http://hz.bjfxy.top/gtjrzlwsez.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jqgfzy.top/gtkzzqikvt.html

[R16] until 等待条件
来源：http://hz.nanxuanxn.top/gteamzvtgg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zycfv.cn/gtwsrjcgcj.html

[R17] 数组定义与取值
来源：http://hz.xingfuxueyuan.xyz/gthztcquwd.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.feifeiyinyue.top/gtnlhqsgro.html

[R18] 遍历数组
来源：http://hz.tanke756.top/gtvgasikzk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.52xcode.cn/gtuhtlgmts.html

[R19] 数组长度
来源：http://hz.bjfxy.top/gtmhsmzdlq.html

echo "${#arr[@]}"
来源：http://hz.ydzc1.top/gtbnhyczkn.html

[R20] 关联数组（字典）
来源：http://hz.ppjwa.cn/gtxgzsvyyl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yuxming.cn/gtzidfgjot.html

[R21] 字符串长度
来源：http://hz.zhijiandao.cn/gtwfhtwmbg.html

echo "${#s}"
来源：http://hz.andypj.xyz/gttzbcivyu.html

[R22] 截取子串
来源：http://hz.fzhhl.top/gtoavoabym.html

echo "${s:0:5}"
来源：http://hz.zhaomingkeji.xyz/gtvkaldsue.html

[R23] 字符串替换
来源：http://hz.jinqigfzy.top/gtvqhstqus.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zdqjudy.top/gtvjzqcxhe.html

[R24] 大小写转换
来源：http://hz.jlsjyb.cn/gtdvfurrwx.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gaohongyu789.top/gthfvfzzvs.html

[R25] 去后缀 / 去前缀
来源：http://hz.xuanzx.com/gtcskdamng.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jyoumei.cn/gtdaxoakex.html

[R26] 命令替换
来源：http://hz.sweek.top/gtbvcumbxi.html

now=$(date +%F); echo "$now"
来源：http://hz.fengsongda.top/gteneypive.html

[R27] 算术展开
来源：http://hz.xuetiantiany.cn/gtyofoigqb.html

echo $((1 + 2 * 3))
来源：http://hz.zhixingplan.top/gtjgufjwes.html

[R28] 浮点运算
来源：http://hz.cdnleiting.top/gtxubvylmt.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinyuanbaomall.cn/gtkxsujzqu.html

[R29] 定义函数
来源：http://hz.jqgufenzy.top/gtlvwvmqlk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shanyushiyangtech.top/gtqvuujfse.html

[R30] 函数返回状态码
来源：http://hz.havefunace.top/gtdbzvhzqr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.kuanghao11.cn/gtmjbnhuds.html

[R31] 局部变量
来源：http://hz.ehwqpu.com/gtehfkmkdh.html

f() { local x=1; echo "$x"; }
来源：http://hz.zdqjudy.top/gtibyqnebp.html

[R32] 参数个数校验
来源：http://hz.kuanghao11.cn/gtmyslccjy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hfpthk.cn/gtchzrzkmj.html

[R33] 捕获错误并提示行号
来源：http://hz.cucudq.cn/gtskhysxaz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tian-w.cn/gtsveuqnjz.html

[R34] 退出时清理
来源：http://hz.52xcode.cn/gtdzmyctru.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnqzz.top/gtiddmmwwp.html

[R35] 后台执行并等待
来源：http://hz.hongshengwenyu.top/gtjskgmajl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.316326.xyz/gtirldivaq.html

[R36] 并发执行多个任务
来源：http://hz.yongpay.top/gteqjtrlsx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jiagoushi.top/gtgiqfggac.html

[R37] 把输出赋给变量
来源：http://hz.cheryme.top/gtanmabiaf.html

files=$(ls -1)
来源：http://hz.zhoulong.xyz/gtcnlvxsoh.html

[R38] 管道串联
来源：http://hz.hongshengwenyu.top/gtjkcgvgqh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shangyingyoupin.top/gtylgdavop.html

[R39] 重定向标准输出与错误
来源：http://hz.cucudq.cn/gthgioboew.html

cmd > out.log 2>&1
来源：http://hz.ydzc1.top/gtinevohub.html

[R40] 追加写日志
来源：http://hz.ivvv.top/gtaursfnpm.html

echo "log" >> out.log
来源：http://hz.ivvv.top/gtxlwnzsai.html

[R41] 丢弃输出
来源：http://hz.wangdashe.top/gtcylfcwlu.html

cmd >/dev/null 2>&1
来源：http://hz.zhoulong.xyz/gtgbvdpicy.html

[R42] 输入重定向
来源：http://hz.daria6918.cn/gtbfhwcpef.html

wc -l < a.txt
来源：http://hz.yuanzhike.top/gtigbkhbqj.html

[R43] 按名字查找文件
来源：http://hz.guannengcc.top/gthwmbzray.html

find . -name "*.log" -type f
来源：http://hz.cashguo.top/gtpfgikomi.html

[R44] 按修改时间查找
来源：http://hz.jinghuilouyu.cn/gtalrkzxtj.html

find . -mtime -7 -type f
来源：http://hz.fengsongda.top/gtwncenerk.html

[R45] 批量删除
来源：http://hz.shanyushiyangtech.top/gtgvpjnfkx.html

find . -name "*.tmp" -delete
来源：http://hz.xuetiantiany.cn/gtuokckorh.html

[R46] 递归替换文件内容
来源：http://hz.xinyue.icu/gtosxfbwqn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nanxuanxn.top/gtbghkudli.html

[R47] sed 单行替换
来源：http://hz.bjfxy.top/gtntdbektj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.wangshuangyany.cn/gtjpiepfyv.html

[R48] awk 取指定列
来源：http://hz.wangshuangyany.cn/gtszoxyqlp.html

awk '{print $1, $3}' a.txt
来源：http://hz.tianlin.xyz/gtbsmmnarz.html

[R49] awk 带条件
来源：http://hz.cdnleiting.top/gttaseavkr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhixingplan.top/gtlqfyobdm.html

[R50] awk 求和
来源：http://hz.daria6918.cn/gtosfmsxoa.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhixingplan.top/gtljmhhxuy.html

[R51] 排序去重取前几
来源：http://hz.fengsongda.top/gtjqjbwifu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ehwqpu.com/gtbrdeofvy.html

[R52] 统计行数
来源：http://hz.zhengqikj.top/gtpwytgwhn.html

wc -l a.txt
来源：http://hz.fzhhl.top/gtplrdigoz.html

[R53] 查看文件头与实时尾
来源：http://hz.bjfxy.top/gtnllzbrzj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.tanke756.top/gtzhwnamgx.html

[R54] 比较两个文件
来源：http://hz.gzhubu.top/gtndwzgxex.html

diff a.txt b.txt
来源：http://hz.redwolf501.top/gtupuujuml.html

[R55] 压缩与解压
来源：http://hz.smart0.xyz/gtfmkwjfey.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.aibaodan.cn/gtugnzulmz.html

[R56] 远程拷贝
来源：http://hz.yueranfly.top/gtjextocyu.html

scp file user@host:/path/
来源：http://hz.gotoacloud.top/gtcaxecyni.html

[R57] 远程执行命令
来源：http://hz.sxryk.cn/gtvmfxmdao.html

ssh user@host 'uptime'
来源：http://hz.hywenlv.cn/gtrfpfniwx.html

[R58] 下载文件
来源：http://hz.chenlongwang.top/gtejrrgvat.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.redwolf501.top/gtiagbjyfp.html

[R59] 发 POST JSON
来源：http://hz.chenjidiqi.icu/gtnrzhxiut.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sysykeji.top/gtjdtygvzi.html

[R60] 只看 HTTP 状态码
来源：http://hz.shanyushiyangkeji.top/gtemodeusk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nanxinkj.top/gtdbrnwimh.html

[R61] 磁盘占用
来源：http://hz.ydjk.org.cn/gtrcxhoiyi.html

df -h;  du -sh *
来源：http://hz.yanxiufei.cn/gtdyalpgav.html

[R62] 找最占空间的文件
来源：http://hz.shanyushiyangtech.top/gtisvltrdf.html

du -ah . | sort -rh | head -10
来源：http://hz.ydzc1.top/gtyghhoyps.html

[R63] 内存与进程
来源：http://hz.aizwys.cn/gtcwwaukjp.html

free -h;  ps aux | grep nginx
来源：http://hz.smart0.xyz/gtlqnurdwv.html

[R64] 结束进程
来源：http://hz.aizwys.cn/gtkgvqtxax.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xinyue.icu/gtpifjewmj.html

[R65] 查看端口占用
来源：http://hz.aibaodan.cn/gtzkffwtzi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.iojbl.cn/gtnxzucqej.html

[R66] 定时任务
来源：http://hz.smart0.xyz/gtpaajjadr.html

crontab -e;  crontab -l
来源：http://hz.xinyue.icu/gtyifwrkrr.html

[R67] 生成随机十六进制串
来源：http://hz.pengpengdd.cyou/gtyvlckxaa.html

openssl rand -hex 16
来源：http://hz.nwbrower.top/gtwyyperlz.html

[R68] 计算文件校验值
来源：http://hz.aibaodan.cn/gtxhbqzpnr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.pycfn.com/gtfwbxepiw.html

[R69] 生成随机密码
来源：http://hz.aibaodan.cn/gtnjdvbvnw.html

head -c 16 /dev/urandom | base64
来源：http://hz.zycfv.cn/gtobkbrmdm.html

[R70] 时间戳与互转
来源：http://hz.cdnleiting.top/gtjdpbykua.html

date +%s;  date -d @1700000000
来源：http://hz.kuanghao11.cn/gtfsxrjudf.html

[R71] 日期格式化
来源：http://hz.zhixingplan.top/gtxcqcxtps.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinghuilouyu.cn/gtsbrvtkzl.html

[R72] 等待端口就绪
来源：http://hz.chenjidiqi.icu/gtcfozombs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cucudq.cn/gterieamoa.html

[R73] 分割大日志
来源：http://hz.nanxuanxn.top/gtmzwfmwzv.html

split -l 1000 big.log part_
来源：http://hz.yj20258.top/gtjoawquhl.html

[R74] 批量重命名
来源：http://hz.yanxiufei.cn/gtnohxijru.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.nanxuanxn.top/gtzmqqrghg.html

[R75] 导出环境变量
来源：http://hz.jyoumei.cn/gtdwqgoldo.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.aizwys.cn/gtltjsdmtg.html

[R76] 使用临时文件
来源：http://hz.xziqi.cn/gttguorpss.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtxlpckikh.html

[R77] 读取用户输入
来源：http://hz.haohaochexian.top/gthluxsrwj.html

read -rp "请输入: " ans
来源：http://hz.yuanzhike.top/gttxcmjmah.html

[R78] 交互式菜单
来源：http://hz.jlsjyb.cn/gtxdwgvius.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.52xcode.cn/gtvftbqmen.html

[R79] 解析命令行选项
来源：http://hz.ywan-chungtsiang.top/gtoiuemnts.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yonumen.top/gtzmukoemv.html

[R80] 查看脚本执行耗时
来源：http://hz.yangfankeji.com/gtdeqekfqu.html

time ./run.sh
来源：http://hz.jinyuanbaomall.cn/gtbocgwmti.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtkqqqtejd.html

S. C / C++ 专题
来源：http://hz.guowangkeji.top/gtglcpbvvb.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtewoprzsu.html

[S01] C：Hello World
来源：http://hz.zhongyouzk.top/gtbcdgjnha.html

#include <stdio.h>
来源：http://hz.sysykeji.top/gtpxotvabl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.fzhhl.top/gtzlblmxnw.html

[S02] C：变量与格式化输出
来源：http://hz.kuanghao11.cn/gtlgheeysr.html

int a = 10; printf("%d\n", a);
来源：http://hz.daxiang520.top/gtuihbdasj.html

[S03] C：读入整数
来源：http://hz.sxryk.cn/gtbyxenbnk.html

int x; scanf("%d", &x);
来源：http://hz.52xcode.cn/gtmqegemez.html

[S04] C：字符串复制
来源：http://hz.shzxlz.cn/gtytxwtdij.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hysaishi.cn/gtuoeviuwu.html

[S05] C：字符串长度
来源：http://hz.fengsongda.top/gtzmyrimgz.html

strlen(s)
来源：http://hz.zycfv.cn/gtusggtuui.html

[S06] C：字符串比较
来源：http://hz.nwbrower.top/gtubyuaomj.html

strcmp(a, b) == 0
来源：http://hz.vqdsnc.cn/gtmpnbtyei.html

[S07] C：数组遍历求和
来源：http://hz.cdnleiting.top/gtzquqciwu.html


<!-- 参考信息 -->