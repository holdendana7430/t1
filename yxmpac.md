代发 wailian999

[Q36] 左连接
来源：http://hz.tanke756.top/gtmjbcgsww.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sufxvd.cn/gtxoiuiwxr.html

[Q37] 右连接
来源：http://hz.mhx1999.top/gtadmicjko.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yvedp.cn/gtipnuelqs.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fzhhl.top/gtlzpjejdk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xylfe.cn/gteggpuajs.html

[Q39] 自连接（查上下级）
来源：http://hz.xziqi.cn/gtajegwaiq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shzxlz.cn/gtdpgxhbgc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.bjfxy.top/gtfrwjiygl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cqqwz.cn/gtrpbwhmjd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yvedp.cn/gtliapypnq.html

[Q41] 多表连接
来源：http://hz.ehwqpu.com/gtfwnkufnq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.fengsongda.top/gttaubkcyo.html

JOIN users u ON u.id = o.user_id
来源：http://hz.tian-w.cn/gtfaxqwxgx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cdnleiting.top/gthvmobbqq.html

[Q42] 连接条件附加过滤
来源：http://hz.xinyue.icu/gtmhnpqvri.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cashguo.top/gtkfhobesr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhijiandao.cn/gtrlbhwjvr.html

[Q43] 标量子查询
来源：http://hz.zhixingplan.top/gtpzqhuxql.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.316326.xyz/gtddhngckb.html

[Q44] IN 子查询
来源：http://hz.nwbrower.top/gteoqbmpoh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shuidangran.top/gtsgctruhg.html

[Q45] EXISTS 判断存在
来源：http://hz.hysaishi.cn/gtvniriqxl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gzhubu.top/gtswxuavdx.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hnxiangtu.top/gtbhkrajco.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zdqjudy.top/gtbldlshki.html

[Q47] 与平均值比较
来源：http://hz.sufxvd.cn/gtwaksggjw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xuanzx.com/gtdnrsebms.html

[Q48] CTE 公用表表达式
来源：http://hz.yanxiufei.cn/gtdnkmbksv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gogol.net.cn/gtikirtpdh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tianlin.xyz/gtbhagftdy.html

[Q49] 更新单行
来源：http://hz.dianchejie.cn/gtsqfuhgkb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.feifeiyinyue.top/gtrghiyind.html

[Q50] 批量更新
来源：http://hz.shangyingyoupin.top/gtsnrjjqtp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhijiandao.cn/gtwdpvlfmh.html

[Q51] 用子查询更新
来源：http://hz.guowangkeji.top/gtlizdwtaf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zycfv.cn/gtbfnpmkbv.html

[Q52] 删除指定行
来源：http://hz.sxryk.cn/gtwbntqfzv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sweek.top/gtoutqhmqf.html

[Q53] 按条件删除
来源：http://hz.nanxinkj.top/gtbbhbymwh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.chenzaomai.com/gtjremkpxx.html

[Q54] 清空表
来源：http://hz.fengsongda.top/gtvskcqkoi.html

TRUNCATE TABLE logs;
来源：http://hz.xuanzx.com/gtmyaktpsd.html

[Q55] 排名（并列占位）
来源：http://hz.fengsongda.top/gtyudjwsxg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yueranfly.top/gtgeijkqhw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.guowangkeji.top/gthxtipsvm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yuxming.cn/gtskaewrod.html

[Q57] 行号
来源：http://hz.aizwys.cn/gthdunfvhz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.chenzaomai.com/gthiocmeje.html

[Q58] 累计求和
来源：http://hz.ybcxt.top/gtjmmydvsa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtcgxledmp.html

[Q59] 分组内累计
来源：http://hz.yj20258.top/gtueupenvx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.andypj.xyz/gtmwnastoe.html

[Q60] 取上一行 / 下一行
来源：http://hz.yuanzhike.top/gtlfisudyb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yongpay.top/gteuizqrrw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xuanzx.com/gtdisogxva.html

[Q61] 移动平均
来源：http://hz.vqdsnc.cn/gtodzifwny.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.smart0.xyz/gtnympjaui.html

[Q62] 分组占比
来源：http://hz.yanxiufei.cn/gtyvzstngd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yuxming.cn/gtwqmbntzq.html

[Q63] 开启事务
来源：http://hz.guannengcc.top/gtmbcjrkgc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.daria6918.cn/gtxmhamzwu.html

[Q64] 提交事务
来源：http://hz.jiagoushi.top/gtusdfdmfh.html

COMMIT;
来源：http://hz.meibo888.top/gtwlvjvnyv.html

[Q65] 回滚事务
来源：http://hz.pengpengdd.cyou/gttyhsbupe.html

ROLLBACK;
来源：http://hz.zhixingplan.top/gtdfhflorl.html

[Q66] 行锁查询
来源：http://hz.jinqigufen.top/gtboxfvdme.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hfpthk.cn/gtcxyjemng.html

[Q67] 设置隔离级别
来源：http://hz.xingfuxueyuan.xyz/gtmpulhmuc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yuxming.cn/gtdxtvbkmf.html

[Q68] 保存点
来源：http://hz.shuidangran.top/gtedbkgnaz.html

SAVEPOINT sp1;
来源：http://hz.xingfuxueyuan.xyz/gtgpogqnhm.html

ROLLBACK TO sp1;
来源：http://hz.gaohongyu789.top/gtnjjpefyh.html

[Q69] 查看执行计划
来源：http://hz.meibo888.top/gttwimgreh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yvedp.cn/gtiercpklv.html

[Q70] 更新统计信息
来源：http://hz.zhengqikj.top/gtdwtjorhp.html

ANALYZE TABLE users;
来源：http://hz.yj20258888.top/gtgndeasbn.html

[Q71] 查看建表语句
来源：http://hz.gotoacloud.top/gtbbstgbol.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.smart0.xyz/gtnswvmdfr.html

[Q72] 查看索引
来源：http://hz.sufxvd.cn/gtqxxermre.html

SHOW INDEX FROM users;
来源：http://hz.guannengcc.top/gtgiktflhj.html

[Q73] 查看表状态
来源：http://hz.zhixingplan.top/gtjeoicwln.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hnqzz.top/gtajzxjthp.html

[Q74] 强制使用索引
来源：http://hz.zycfv.cn/gtechsszgo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.meibo888.top/gtccpuyhne.html

[Q75] 日期格式化
来源：http://hz.ydzc1.top/gtmpnfxtyv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xziqi.cn/gtbsrnfjhk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cdnleiting.top/gtzlgshhqu.html

[Q76] 按天统计
来源：http://hz.daxiang520.top/gtjibunrhg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cqqwz.cn/gtvjjtycgw.html

[Q77] 时间加减
来源：http://hz.hnqzz.top/gtktnsqmrs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yuanzhike.top/gtwnwionjo.html

[Q78] 当前时间
来源：http://hz.svipenyu.cn/gtxqgwsjfo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhaomingkeji.xyz/gtsadotyve.html

[Q79] 字符串拼接
来源：http://hz.aibaodan.cn/gtqipqxsds.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.svipenyu.cn/gtiiaotqcu.html

[Q80] 字符串截取
来源：http://hz.yuxming.cn/gtjndnbegw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.smart0.xyz/gtdsxwcyyd.html

[Q81] 字符串替换
来源：http://hz.gaohongyu789.top/gtwwkqdpfz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhoulong.xyz/gtxbxsbhwr.html

[Q82] 字符长度与字节长度
来源：http://hz.pycfn.com/gtzcqmrawa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gzhubu.top/gtlbtueabu.html

[Q83] 大小写转换
来源：http://hz.hfpthk.cn/gtecyxnugr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.andypj.xyz/gtrtshltby.html

[Q84] 去除首尾空格
来源：http://hz.xuetiantiany.cn/gtmnnokwcx.html

SELECT TRIM(name) FROM users;
来源：http://hz.ybcxt.top/gtpvkyqlxg.html

[Q85] 数值取整
来源：http://hz.zhengqikj.top/gtsuiewwjb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhaomingkeji.xyz/gtmwvhbdwz.html

[Q86] 读取 JSON 字段
来源：http://hz.nwbrower.top/gtcfrzblke.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhijiandao.cn/gtvbtcsriq.html

[Q87] JSON 字段做条件
来源：http://hz.zhoulong.xyz/gtztbuklui.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj202588.top/gtwtzckgqs.html

[Q88] 行转列（条件聚合）
来源：http://hz.xingfuxueyuan.xyz/gtfbnzukme.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hysaishi.cn/gtdhgxrkjk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.pengpengdd.cyou/gtxgxzobyb.html

[Q89] 判断表是否存在
来源：http://hz.dianchejie.cn/gtyrbiwjqt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.daria6918.cn/gtdmqwgcfg.html

[Q90] 生成序号列
来源：http://hz.haohaochexian.top/gtpqbauujj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hywenlv.cn/gtfliaqhit.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtubbokzvn.html

R. Bash 专题
来源：http://hz.svipenyu.cn/gtacmzvrxy.html

================================================================================
来源：http://hz.gzhubu.top/gtgrpzfspm.html

[R01] shebang 与严格模式
来源：http://hz.hysaishi.cn/gtpunhhpxk.html

#!/usr/bin/env bash
来源：http://hz.meibo888.top/gtlwglviti.html

set -euo pipefail
来源：http://hz.shuidangran.top/gtrverrwxa.html

[R02] 变量赋值与使用
来源：http://hz.ybcxt.top/gtbiiooiyr.html

name="Tom"; echo "$name"
来源：http://hz.jiagoushi.top/gticwwbpqv.html

[R03] 只读变量
来源：http://hz.dianchejie.cn/gtzrteieoo.html

readonly PI=3.14
来源：http://hz.hywenlv.cn/gtnotfhoeg.html

[R04] 位置参数
来源：http://hz.xuanzx.com/gtopcmkito.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.9152youxi.cn/gtdawpticy.html

[R05] 参数默认值
来源：http://hz.hnqzz.top/gtvotemhwt.html

name="${1:-default}"
来源：http://hz.yuxming.cn/gtpncykmuv.html

[R06] 判断命令是否存在
来源：http://hz.dashuyun.cn/gtiuqhipqp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hysaishi.cn/gtumvbkjew.html

[R07] if 判断文件
来源：http://hz.zhijiandao.cn/gtkmgqozpx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinqigufen.top/gtyaurpisk.html

[R08] 数值比较
来源：http://hz.xuanzx.com/gtolghznmr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hysaishi.cn/gtenemjpqs.html

[R09] 字符串比较
来源：http://hz.316326.xyz/gtjkmcxacz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hnqzz.top/gtxjnzxrhm.html

[R10] 正则匹配
来源：http://hz.daria6918.cn/gtqgaszahr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenlongwang.top/gtfcjaduyz.html

[R11] case 多分支
来源：http://hz.zhiwuduotai.top/gtxfoqqrbi.html

case "$1" in
来源：http://hz.bjfxy.top/gtpcixyxaa.html

start) echo "启动" ;;
来源：http://hz.zhaomingkeji.xyz/gtosxplqka.html

stop)  echo "停止" ;;
来源：http://hz.tianlin.xyz/gtsoqfcqfq.html

*)     echo "未知命令" ;;
来源：http://hz.jianghu66.top/gtfwznisoi.html

esac
来源：http://hz.snrcjt.cn/gtvyvbmnzv.html

[R12] for 遍历文件
来源：http://hz.daria6918.cn/gtbdffkevn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.wangshuangyany.cn/gtonamcram.html

[R13] for 计数循环
来源：http://hz.redwolf501.top/gtmecwftiy.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.fzhhl.top/gtjdoswijr.html

[R14] C 风格 for
来源：http://hz.zycfv.cn/gtoyeepisx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hfpthk.cn/gtfsyyvqco.html

[R15] while 逐行读文件
来源：http://hz.svipenyu.cn/gtbjvbsubq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ybcxt.top/gtmwupjydl.html

[R16] until 等待条件
来源：http://hz.quarkkingdee.top/gtuefpcqcy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ydzc1.top/gtmmcpphem.html

[R17] 数组定义与取值
来源：http://hz.nwbrower.top/gtbynhirvc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aibaodan.cn/gttfjlrqlp.html

[R18] 遍历数组
来源：http://hz.zhaomingkeji.xyz/gtgsaabbzk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinqigfzy.top/gtxawnknfn.html

[R19] 数组长度
来源：http://hz.0kj1m.cn/gtqsrnmuce.html

echo "${#arr[@]}"
来源：http://hz.snrcjt.cn/gtohfqugdk.html

[R20] 关联数组（字典）
来源：http://hz.hongshengwenyu.top/gtniolrfxt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sweek.top/gtwkffevas.html

[R21] 字符串长度
来源：http://hz.yangfankeji.com/gtqxidrizl.html

echo "${#s}"
来源：http://hz.yuanzhike.top/gtmuunzevo.html

[R22] 截取子串
来源：http://hz.ppjwa.cn/gtqsmaxkeb.html

echo "${s:0:5}"
来源：http://hz.hongshengwenyu.top/gtistvwdjk.html

[R23] 字符串替换
来源：http://hz.gotoacloud.top/gtnafrxjmt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.chenlongwang.top/gtjrxcifpu.html

[R24] 大小写转换
来源：http://hz.52xcode.cn/gtywyccfkz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenzaomai.com/gttsxlppoq.html

[R25] 去后缀 / 去前缀
来源：http://hz.cashguo.top/gtxbsvfeks.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jiagoushi.top/gtkepnodxk.html

[R26] 命令替换
来源：http://hz.redwolf501.top/gtpoyjeddx.html

now=$(date +%F); echo "$now"
来源：http://hz.nanxuanxn.top/gtlbdqjace.html

[R27] 算术展开
来源：http://hz.dashuyun.cn/gtllfozeos.html

echo $((1 + 2 * 3))
来源：http://hz.dianchejie.cn/gtccpfasbl.html

[R28] 浮点运算
来源：http://hz.xylfe.cn/gtucpfhlpz.html

echo "scale=2; 10/3" | bc
来源：http://hz.52xcode.cn/gtqqmonzsv.html

[R29] 定义函数
来源：http://hz.jinqigfzy.top/gtgqhurqxy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hammf.cn/gthrkqzulp.html

[R30] 函数返回状态码
来源：http://hz.jqgufenzy.top/gttvkguvfh.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.iojbl.cn/gttbjjunfq.html

[R31] 局部变量
来源：http://hz.shangyingyoupin.top/gttnmejmib.html

f() { local x=1; echo "$x"; }
来源：http://hz.9152youxi.cn/gtjeqqdujx.html

[R32] 参数个数校验
来源：http://hz.0kj1m.cn/gtwwqmledk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinqigfzy.top/gtelorlird.html

[R33] 捕获错误并提示行号
来源：http://hz.zhengqikj.top/gtxgkljmql.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jqgfzy.top/gtttnbkrsb.html

[R34] 退出时清理
来源：http://hz.zhoulong.xyz/gtciqvczhu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sysykeji.top/gtwgygejsh.html

[R35] 后台执行并等待
来源：http://hz.dashuyun.cn/gtiejoqrxg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cdnleiting.top/gtlkafdymu.html

[R36] 并发执行多个任务
来源：http://hz.yj202588.top/gtzpvkctox.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.daria6918.cn/gtzghtdhql.html

[R37] 把输出赋给变量
来源：http://hz.fengsongda.top/gtvwxtxwsd.html

files=$(ls -1)
来源：http://hz.jianghu66.top/gtfdpaayea.html

[R38] 管道串联
来源：http://hz.hfpthk.cn/gtsjldmtqy.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xingfuxueyuan.xyz/gttbvbnmfu.html

[R39] 重定向标准输出与错误
来源：http://hz.nanxuanxn.top/gtbzsiogwl.html

cmd > out.log 2>&1
来源：http://hz.sysykeji.top/gtxsmaianq.html

[R40] 追加写日志
来源：http://hz.9152youxi.cn/gtaxnpkbdy.html

echo "log" >> out.log
来源：http://hz.kuanghao11.cn/gtyharizaj.html

[R41] 丢弃输出
来源：http://hz.nanxinkj.top/gtlybottwf.html

cmd >/dev/null 2>&1
来源：http://hz.jinghuilouyu.cn/gtvfmzszki.html

[R42] 输入重定向
来源：http://hz.chenzaomai.com/gtaglupfcc.html

wc -l < a.txt
来源：http://hz.pengpengdd.cyou/gtkxphjnay.html

[R43] 按名字查找文件
来源：http://hz.sxryk.cn/gtoxuwgjyn.html

find . -name "*.log" -type f
来源：http://hz.smart0.xyz/gtpnccovgq.html

[R44] 按修改时间查找
来源：http://hz.shuidangran.top/gtxjdeulyi.html

find . -mtime -7 -type f
来源：http://hz.xingfuxueyuan.xyz/gtkvmskafs.html

[R45] 批量删除
来源：http://hz.iojbl.cn/gtcefmcqyz.html

find . -name "*.tmp" -delete
来源：http://hz.jinghuilouyu.cn/gtvyxotzxv.html

[R46] 递归替换文件内容
来源：http://hz.daria6918.cn/gtaofytxfq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cheryme.top/gtdoupejoa.html

[R47] sed 单行替换
来源：http://hz.jinghuilouyu.cn/gtmjdojmru.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sysykeji.top/gtwkcofhjz.html

[R48] awk 取指定列
来源：http://hz.pycfn.com/gteiwvascb.html

awk '{print $1, $3}' a.txt
来源：http://hz.xuetiantiany.cn/gtoejxncev.html

[R49] awk 带条件
来源：http://hz.xingfuxueyuan.xyz/gtikcbecnl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.iojbl.cn/gtjmarerau.html

[R50] awk 求和
来源：http://hz.ppjwa.cn/gtqoqmuwkq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhongyouzk.top/gtcuhihbyi.html

[R51] 排序去重取前几
来源：http://hz.52xcode.cn/gtmusrarlp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gaohongyu789.top/gtmiohlfez.html

[R52] 统计行数
来源：http://hz.guannengcc.top/gtvlejkmwj.html

wc -l a.txt
来源：http://hz.mhx1999.top/gtyeqnmxrn.html

[R53] 查看文件头与实时尾
来源：http://hz.hnxiangtu.top/gtapiocxxs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.tianlin.xyz/gtxzsuncbf.html

[R54] 比较两个文件
来源：http://hz.shangyingyoupin.top/gtkdpbczgw.html

diff a.txt b.txt
来源：http://hz.wangshuangyany.cn/gtjoostcga.html

[R55] 压缩与解压
来源：http://hz.havefunace.top/gtuainejqi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ppjwa.cn/gtfotaqrrt.html

[R56] 远程拷贝
来源：http://hz.mhx1999.top/gthntaemox.html

scp file user@host:/path/
来源：http://hz.havefunace.top/gtbnstyhxp.html

[R57] 远程执行命令
来源：http://hz.chenjidiqi.icu/gtaeljvldd.html

ssh user@host 'uptime'
来源：http://hz.zycfv.cn/gtoqardewr.html

[R58] 下载文件
来源：http://hz.hammf.cn/gtpyokxknu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.c1oappe.top/gtutjfuxqc.html

[R59] 发 POST JSON
来源：http://hz.cashguo.top/gtfimzihpl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.chenjidiqi.icu/gtzzaqblsl.html

[R60] 只看 HTTP 状态码
来源：http://hz.iojbl.cn/gtrnnoaiga.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jiagoushi.top/gtoqwfedyn.html

[R61] 磁盘占用
来源：http://hz.fzhhl.top/gtvplauhqg.html

df -h;  du -sh *
来源：http://hz.hfpthk.cn/gtbkrxydvn.html

[R62] 找最占空间的文件
来源：http://hz.birdmap.top/gtadhtpuun.html

du -ah . | sort -rh | head -10
来源：http://hz.hysaishi.cn/gtwcoarsfo.html

[R63] 内存与进程
来源：http://hz.chenjidiqi.icu/gtrgpoekjp.html

free -h;  ps aux | grep nginx
来源：http://hz.ydzc1.top/gtfhcuijky.html

[R64] 结束进程
来源：http://hz.zdqjudy.top/gtqtrxbpfl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.pycfn.com/gtkmkzxibx.html

[R65] 查看端口占用
来源：http://hz.yangfankeji.com/gtaxupsksu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.smart0.xyz/gtwpiuntgj.html

[R66] 定时任务
来源：http://hz.xylfe.cn/gtlkxqfevm.html

crontab -e;  crontab -l
来源：http://hz.hysaishi.cn/gtrzcoosnd.html

[R67] 生成随机十六进制串
来源：http://hz.shanyushiyangtech.top/gtvzqsovcm.html

openssl rand -hex 16
来源：http://hz.sweek.top/gtduhwzjfm.html

[R68] 计算文件校验值
来源：http://hz.tanke756.top/gthuubzzne.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jqgfzy.top/gtkepvtlnb.html

[R69] 生成随机密码
来源：http://hz.cqqwz.cn/gtkaccrdgw.html

head -c 16 /dev/urandom | base64
来源：http://hz.zdqjudy.top/gtzzwaafkj.html

[R70] 时间戳与互转
来源：http://hz.shuidangran.top/gtaukdqfda.html

date +%s;  date -d @1700000000
来源：http://hz.ywan-chungtsiang.top/gttuuyixqw.html

[R71] 日期格式化
来源：http://hz.haohaochexian.top/gtljstsjyt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinyuanbaomall.cn/gtyvdcimke.html

[R72] 等待端口就绪
来源：http://hz.meibo888.top/gtqpgdggsd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhongyouzk.top/gtfxujtdmv.html

[R73] 分割大日志
来源：http://hz.sufxvd.cn/gtcyhkcgum.html

split -l 1000 big.log part_
来源：http://hz.cdnleiting.top/gtznznujee.html

[R74] 批量重命名
来源：http://hz.iojbl.cn/gtdvodhltc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.bjfxy.top/gtglvbrpmh.html

[R75] 导出环境变量
来源：http://hz.yj202588.top/gtjmtsqxpg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cheryme.top/gtzlkdjnit.html

[R76] 使用临时文件
来源：http://hz.tianlin.xyz/gtxlpwjxzi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnxiangtu.top/gtxfylskff.html

[R77] 读取用户输入
来源：http://hz.andypj.xyz/gttfuuuggq.html

read -rp "请输入: " ans
来源：http://hz.aibaodan.cn/gtatdbdtov.html

[R78] 交互式菜单
来源：http://hz.shanyushiyangkeji.top/gthmqjyrdk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.wangdashe.top/gtuquxqosp.html

[R79] 解析命令行选项
来源：http://hz.zycfv.cn/gtpvltdwll.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sweek.top/gtpyjuktql.html

[R80] 查看脚本执行耗时
来源：http://hz.hammf.cn/gtrcprloey.html

time ./run.sh
来源：http://hz.cqqwz.cn/gtpxnbodoh.html

================================================================================
来源：http://hz.kuanghao11.cn/gtisczsmkz.html

S. C / C++ 专题
来源：http://hz.jyoumei.cn/gtjdfsukgx.html

================================================================================
来源：http://hz.yanxiufei.cn/gtpzqpshwc.html

[S01] C：Hello World
来源：http://hz.zhengqikj.top/gtpzufqcdv.html

#include <stdio.h>
来源：http://hz.jinqigfzy.top/gtepyrhenu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.316326.xyz/gtbfakylrh.html

[S02] C：变量与格式化输出
来源：http://hz.yanxiufei.cn/gtrphzfnzp.html

int a = 10; printf("%d\n", a);
来源：http://hz.xinyue.icu/gttydyxhxw.html

[S03] C：读入整数
来源：http://hz.nanxinkj.top/gtsuspkgst.html

int x; scanf("%d", &x);
来源：http://hz.cqqwz.cn/gthxmehlad.html

[S04] C：字符串复制
来源：http://hz.yj20258888.top/gtqrkhcfpu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xziqi.cn/gtkgcdzwnz.html

[S05] C：字符串长度
来源：http://hz.xziqi.cn/gtpslyfppg.html


<!-- 参考信息 -->