代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinqigfzy.top/gtawrougpa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.birdmap.top/gtxcxiodla.html

[Q39] 自连接（查上下级）
来源：http://hz.hammf.cn/gtwgtwjiue.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinyuanbaomall.cn/gtminyupqh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.aibaodan.cn/gtgufsdhkw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shanyushiyangkeji.top/gtvignnpsh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shuidangran.top/gtzdqczprq.html

[Q41] 多表连接
来源：http://hz.xziqi.cn/gtwnlojhaz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shanyushiyangtech.top/gtcxtzqvce.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhiwuduotai.top/gtowjgaadu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.aibaodan.cn/gtgdzotmjt.html

[Q42] 连接条件附加过滤
来源：http://hz.mhx1999.top/gtjtcdkryt.html

SELECT u.name, o.amount FROM users u
来源：http://hz.52xcode.cn/gtdeaqqvou.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhaomingkeji.xyz/gtwhhrfeyl.html

[Q43] 标量子查询
来源：http://hz.cashguo.top/gtybdehemc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.pycfn.com/gtdnyuvude.html

[Q44] IN 子查询
来源：http://hz.guannengcc.top/gtslrujkvd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ybcxt.top/gttzbuawku.html

[Q45] EXISTS 判断存在
来源：http://hz.sufxvd.cn/gtsfzjrkel.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuanzhike.top/gtckigkdkv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jqgfzy.top/gttuyucaas.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nwbrower.top/gtdaigxvqy.html

[Q47] 与平均值比较
来源：http://hz.0kj1m.cn/gtmfqxakav.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.aizwys.cn/gtodrzgbao.html

[Q48] CTE 公用表表达式
来源：http://hz.yuxming.cn/gtmtlqfmlh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jqgfzy.top/gtxtdandtn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.aizwys.cn/gtlhtvzyti.html

[Q49] 更新单行
来源：http://hz.gzhubu.top/gtjrcuzqtp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shuidangran.top/gtojdrxbpr.html

[Q50] 批量更新
来源：http://hz.mhx1999.top/gthhonzxcf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.feifeiyinyue.top/gtlnakprvz.html

[Q51] 用子查询更新
来源：http://hz.guowangkeji.top/gtdlpyfxrt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gzhubu.top/gtihczppgf.html

[Q52] 删除指定行
来源：http://hz.dashuyun.cn/gtwovjfwfr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.mhx1999.top/gttbzgqxun.html

[Q53] 按条件删除
来源：http://hz.cashguo.top/gtrbnfrwjc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.52xcode.cn/gtwrsdrcqw.html

[Q54] 清空表
来源：http://hz.zhongyouzk.top/gthekxiwpv.html

TRUNCATE TABLE logs;
来源：http://hz.zdqjudy.top/gtzfiqxyrr.html

[Q55] 排名（并列占位）
来源：http://hz.zhijiandao.cn/gtssfrrbzh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhengqikj.top/gtjaceaznv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.wangdashe.top/gtwutrhdrk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ydjk.org.cn/gtuabhsuaz.html

[Q57] 行号
来源：http://hz.chenlongwang.top/gtajkevsur.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ydjk.org.cn/gtsokaodbh.html

[Q58] 累计求和
来源：http://hz.xziqi.cn/gtykndocvb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.iojbl.cn/gtyktwrwvx.html

[Q59] 分组内累计
来源：http://hz.feifeiyinyue.top/gtapronrri.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.aizwys.cn/gtrnzwcmvf.html

[Q60] 取上一行 / 下一行
来源：http://hz.cheryme.top/gttdxilfjg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jlsjyb.cn/gtkvlzwsvo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xinyue.icu/gthdkmkpov.html

[Q61] 移动平均
来源：http://hz.yongpay.top/gtmsqrfhai.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.dashuyun.cn/gtndlxticf.html

[Q62] 分组占比
来源：http://hz.ywan-chungtsiang.top/gtxonqppop.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.nwbrower.top/gtmrpddwts.html

[Q63] 开启事务
来源：http://hz.hammf.cn/gthtcuzvjf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.redwolf501.top/gtdobbrvxz.html

[Q64] 提交事务
来源：http://hz.guowangkeji.top/gtlylqxoct.html

COMMIT;
来源：http://hz.yangfankeji.com/gtyruujvhu.html

[Q65] 回滚事务
来源：http://hz.smart0.xyz/gtlgpzknwr.html

ROLLBACK;
来源：http://hz.jyoumei.cn/gtyqsxczbs.html

[Q66] 行锁查询
来源：http://hz.zhiwuduotai.top/gtqxoacjrf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ywan-chungtsiang.top/gtdnxikool.html

[Q67] 设置隔离级别
来源：http://hz.ehwqpu.com/gtcmdxwjbm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ehwqpu.com/gtvfgpnpiw.html

[Q68] 保存点
来源：http://hz.0kj1m.cn/gtnjozmhkb.html

SAVEPOINT sp1;
来源：http://hz.zhixingplan.top/gtikfrgvgq.html

ROLLBACK TO sp1;
来源：http://hz.sweek.top/gtloqdmiag.html

[Q69] 查看执行计划
来源：http://hz.cdnleiting.top/gtpwklznft.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinyuanbaomall.cn/gtkpbxnjgn.html

[Q70] 更新统计信息
来源：http://hz.316326.xyz/gtzdstywkc.html

ANALYZE TABLE users;
来源：http://hz.haohaochexian.top/gtemmrrpfa.html

[Q71] 查看建表语句
来源：http://hz.zhijiandao.cn/gtnnxvsvdn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenzaomai.com/gtcfpmxmqe.html

[Q72] 查看索引
来源：http://hz.cqqwz.cn/gtkpwkqqsy.html

SHOW INDEX FROM users;
来源：http://hz.jiagoushi.top/gtxfpwzlgr.html

[Q73] 查看表状态
来源：http://hz.kuanghao11.cn/gtuzqzoyan.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nanxuanxn.top/gtrforiorl.html

[Q74] 强制使用索引
来源：http://hz.havefunace.top/gtotiknrgq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.vqdsnc.cn/gtxrhbhgao.html

[Q75] 日期格式化
来源：http://hz.zhijiandao.cn/gtxqhlynxd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cqqwz.cn/gtinakbxjn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yueranfly.top/gtkscpztwj.html

[Q76] 按天统计
来源：http://hz.yj20258888.top/gtnlyuwycv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ivvv.top/gtptiqexdx.html

[Q77] 时间加减
来源：http://hz.fzhhl.top/gtlsatyktt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cashguo.top/gtgdeaeihg.html

[Q78] 当前时间
来源：http://hz.zycfv.cn/gttifhvlun.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.kuanghao11.cn/gtjirrzegc.html

[Q79] 字符串拼接
来源：http://hz.xylfe.cn/gttnklnbpk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.redwolf501.top/gtdileohlk.html

[Q80] 字符串截取
来源：http://hz.gaohongyu789.top/gtkzjjqzen.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hfpthk.cn/gtqtwxlpck.html

[Q81] 字符串替换
来源：http://hz.jiagoushi.top/gtmgsovvhw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sysykeji.top/gtktmtnouh.html

[Q82] 字符长度与字节长度
来源：http://hz.guannengcc.top/gtxouxayxh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.aizwys.cn/gtizdawqml.html

[Q83] 大小写转换
来源：http://hz.zhoulong.xyz/gtaznlywnz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.snrcjt.cn/gtpfrnkvhd.html

[Q84] 去除首尾空格
来源：http://hz.nanxuanxn.top/gtlfvcnifv.html

SELECT TRIM(name) FROM users;
来源：http://hz.dashuyun.cn/gtzznmqdnu.html

[Q85] 数值取整
来源：http://hz.gzhubu.top/gtnincpdwr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.sufxvd.cn/gthejbjxqi.html

[Q86] 读取 JSON 字段
来源：http://hz.wangshuangyany.cn/gtssnmzzra.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.wangdashe.top/gtjieqntmy.html

[Q87] JSON 字段做条件
来源：http://hz.aibaodan.cn/gtjwwolubu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.daria6918.cn/gteqbjqjsm.html

[Q88] 行转列（条件聚合）
来源：http://hz.fengsongda.top/gtelqmgfhi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.0kj1m.cn/gthxjyzzhy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhongyouzk.top/gtslvxtquo.html

[Q89] 判断表是否存在
来源：http://hz.fzhhl.top/gtjhauxkag.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shanyushiyangkeji.top/gtrrojcchp.html

[Q90] 生成序号列
来源：http://hz.jinghuilouyu.cn/gtclhpvgms.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jianghu66.top/gtugjtxaiv.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gthtyrtqqq.html

R. Bash 专题
来源：http://hz.cdnleiting.top/gtzlpqired.html

================================================================================
来源：http://hz.gogol.net.cn/gtyooaknaw.html

[R01] shebang 与严格模式
来源：http://hz.guowangkeji.top/gtsgwinkby.html

#!/usr/bin/env bash
来源：http://hz.hnxiangtu.top/gtshdkhwru.html

set -euo pipefail
来源：http://hz.ydzc1.top/gtuburrsor.html

[R02] 变量赋值与使用
来源：http://hz.yuanzhike.top/gtiklhwqou.html

name="Tom"; echo "$name"
来源：http://hz.yueranfly.top/gtcxrrkbcx.html

[R03] 只读变量
来源：http://hz.zhoulong.xyz/gtyuktauqk.html

readonly PI=3.14
来源：http://hz.jianghu66.top/gtpsxuqccf.html

[R04] 位置参数
来源：http://hz.cqqwz.cn/gtugopgrvf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.guannengcc.top/gtfditwzja.html

[R05] 参数默认值
来源：http://hz.hywenlv.cn/gtlwtdtuhg.html

name="${1:-default}"
来源：http://hz.shanyushiyangtech.top/gtvhijzgsu.html

[R06] 判断命令是否存在
来源：http://hz.hnxiangtu.top/gtkylytrpb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gaohongyu789.top/gtkhctszmu.html

[R07] if 判断文件
来源：http://hz.chenjidiqi.icu/gtknhpqnbn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.wangshuangyany.cn/gtznsetteo.html

[R08] 数值比较
来源：http://hz.jianghu66.top/gtcrqnldgf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gaohongyu789.top/gtrtxnrlye.html

[R09] 字符串比较
来源：http://hz.sysykeji.top/gtgeagogmv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zdqjudy.top/gteazemsbm.html

[R10] 正则匹配
来源：http://hz.aizwys.cn/gttizsmhrd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.andypj.xyz/gtoqiwabsh.html

[R11] case 多分支
来源：http://hz.nwbrower.top/gtisssjbdg.html

case "$1" in
来源：http://hz.gaohongyu789.top/gtooyekmpu.html

start) echo "启动" ;;
来源：http://hz.andypj.xyz/gtlxvkslyi.html

stop)  echo "停止" ;;
来源：http://hz.zhiwuduotai.top/gtbaktmeae.html

*)     echo "未知命令" ;;
来源：http://hz.svipenyu.cn/gtjsvkrbas.html

esac
来源：http://hz.yj202588.top/gtjlbujdkg.html

[R12] for 遍历文件
来源：http://hz.jlsjyb.cn/gtvzjgfknu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.birdmap.top/gtxeqaoixz.html

[R13] for 计数循环
来源：http://hz.cashguo.top/gtgytqysiw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gotoacloud.top/gtpcsbxfij.html

[R14] C 风格 for
来源：http://hz.jinyuanbaomall.cn/gttsxvivbe.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.fzhhl.top/gtwqgarjli.html

[R15] while 逐行读文件
来源：http://hz.yanxiufei.cn/gtuqwolhdw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sufxvd.cn/gtetsqkrre.html

[R16] until 等待条件
来源：http://hz.zycfv.cn/gtvobgahua.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtovkatuom.html

[R17] 数组定义与取值
来源：http://hz.gogol.net.cn/gteymxbxje.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gaohongyu789.top/gtwlrgpcga.html

[R18] 遍历数组
来源：http://hz.fzhhl.top/gtakluavns.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jqgfzy.top/gtmkbkeobw.html

[R19] 数组长度
来源：http://hz.jqgfzy.top/gtwbaapspb.html

echo "${#arr[@]}"
来源：http://hz.yongpay.top/gtjgeayklv.html

[R20] 关联数组（字典）
来源：http://hz.jinghuilouyu.cn/gtyiexhfgr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj20258888.top/gtiyclvptq.html

[R21] 字符串长度
来源：http://hz.zhaomingkeji.xyz/gtixmlcbdr.html

echo "${#s}"
来源：http://hz.ybcxt.top/gtwgknbmlo.html

[R22] 截取子串
来源：http://hz.fengsongda.top/gttzxpwtpp.html

echo "${s:0:5}"
来源：http://hz.zhoulong.xyz/gtzynvmfhi.html

[R23] 字符串替换
来源：http://hz.c1oappe.top/gtfvjbdjae.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ydzc1.top/gtscxbeqyr.html

[R24] 大小写转换
来源：http://hz.andypj.xyz/gtuhqreyxx.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj202588.top/gtpjsdiczj.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinqigufen.top/gtuzthrqht.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gzhubu.top/gtswlyqtyn.html

[R26] 命令替换
来源：http://hz.fengsongda.top/gtphkmxudn.html

now=$(date +%F); echo "$now"
来源：http://hz.cqqwz.cn/gtfjojzqfq.html

[R27] 算术展开
来源：http://hz.dianchejie.cn/gtkdiutpxz.html

echo $((1 + 2 * 3))
来源：http://hz.wangdashe.top/gtujpwiqmc.html

[R28] 浮点运算
来源：http://hz.316326.xyz/gttaxgbqfa.html

echo "scale=2; 10/3" | bc
来源：http://hz.tian-w.cn/gtfwnquuwm.html

[R29] 定义函数
来源：http://hz.52xcode.cn/gtilmvtdek.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yangfankeji.com/gtuxmvpvyn.html

[R30] 函数返回状态码
来源：http://hz.andypj.xyz/gtcchowvyp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yueranfly.top/gtlckzdadq.html

[R31] 局部变量
来源：http://hz.jiagoushi.top/gthnxonhor.html

f() { local x=1; echo "$x"; }
来源：http://hz.hywenlv.cn/gtbeqzcyws.html

[R32] 参数个数校验
来源：http://hz.guannengcc.top/gtwpckcquo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yongpay.top/gthebjqhtp.html

[R33] 捕获错误并提示行号
来源：http://hz.redwolf501.top/gtmxkjkjgr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ppjwa.cn/gtaorhblrs.html

[R34] 退出时清理
来源：http://hz.zhijiandao.cn/gtkytvbszj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.aibaodan.cn/gtsyyzdoxv.html

[R35] 后台执行并等待
来源：http://hz.smart0.xyz/gtcuejbtuh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhijiandao.cn/gtvfoavbaw.html

[R36] 并发执行多个任务
来源：http://hz.nanxuanxn.top/gtkxmfchpg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.haohaochexian.top/gtldvdlvul.html

[R37] 把输出赋给变量
来源：http://hz.gzhubu.top/gtncspxdbp.html

files=$(ls -1)
来源：http://hz.havefunace.top/gtszerquzg.html

[R38] 管道串联
来源：http://hz.hywenlv.cn/gtepspggxt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.snrcjt.cn/gtsultxsqr.html

[R39] 重定向标准输出与错误
来源：http://hz.feifeiyinyue.top/gtrsbbtaum.html

cmd > out.log 2>&1
来源：http://hz.316326.xyz/gtrtwhhwnz.html

[R40] 追加写日志
来源：http://hz.hysaishi.cn/gtjijmhips.html

echo "log" >> out.log
来源：http://hz.hywenlv.cn/gtecpfvpix.html

[R41] 丢弃输出
来源：http://hz.daxiang520.top/gtafrsjnkw.html

cmd >/dev/null 2>&1
来源：http://hz.zhongyouzk.top/gtltbzehky.html

[R42] 输入重定向
来源：http://hz.ydzc1.top/gtzzsuyibn.html

wc -l < a.txt
来源：http://hz.zdqjudy.top/gtdnarvmyd.html

[R43] 按名字查找文件
来源：http://hz.zdqjudy.top/gtbzdlmegq.html

find . -name "*.log" -type f
来源：http://hz.ppjwa.cn/gtestbjxwf.html

[R44] 按修改时间查找
来源：http://hz.0kj1m.cn/gtpyzqkdum.html

find . -mtime -7 -type f
来源：http://hz.yanxiufei.cn/gtbptojuwo.html

[R45] 批量删除
来源：http://hz.jiagoushi.top/gtfnntjctq.html

find . -name "*.tmp" -delete
来源：http://hz.gogol.net.cn/gtpcumeyst.html

[R46] 递归替换文件内容
来源：http://hz.cucudq.cn/gtlxhrvlwr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.c1oappe.top/gtgiflzxyj.html

[R47] sed 单行替换
来源：http://hz.yanxiufei.cn/gtvmuonjsr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.snrcjt.cn/gtitoralrx.html

[R48] awk 取指定列
来源：http://hz.hnqzz.top/gtxaerpvju.html

awk '{print $1, $3}' a.txt
来源：http://hz.ywan-chungtsiang.top/gtelrkbghj.html

[R49] awk 带条件
来源：http://hz.cheryme.top/gtiipuxmaf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ywan-chungtsiang.top/gtwjepphdd.html

[R50] awk 求和
来源：http://hz.hysaishi.cn/gtkkwpkogk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xinyue.icu/gtsjwnphif.html

[R51] 排序去重取前几
来源：http://hz.haohaochexian.top/gtlhukyzbo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydzc1.top/gtvjggmwuw.html

[R52] 统计行数
来源：http://hz.xziqi.cn/gtrejxjrsa.html

wc -l a.txt
来源：http://hz.jqgufenzy.top/gtfiuonqyn.html

[R53] 查看文件头与实时尾
来源：http://hz.cheryme.top/gtdjggybvv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.0kj1m.cn/gtcunfhkqb.html

[R54] 比较两个文件
来源：http://hz.svipenyu.cn/gtdaavyqss.html

diff a.txt b.txt
来源：http://hz.aizwys.cn/gtdzdjwelw.html

[R55] 压缩与解压
来源：http://hz.jinqigfzy.top/gtgkfsxxhy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhongyouzk.top/gtyesecvso.html

[R56] 远程拷贝
来源：http://hz.yuanzhike.top/gtoftcrbqb.html

scp file user@host:/path/
来源：http://hz.hongshengwenyu.top/gtnwcgtbuf.html

[R57] 远程执行命令
来源：http://hz.xuetiantiany.cn/gtksavcpyj.html

ssh user@host 'uptime'
来源：http://hz.yonumen.top/gtyusozsee.html

[R58] 下载文件
来源：http://hz.sxryk.cn/gtfjzstjpb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.pengpengdd.cyou/gtxqvnhzuu.html

[R59] 发 POST JSON
来源：http://hz.guowangkeji.top/gtijfqjbhy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ydzc1.top/gtxhbsimiu.html

[R60] 只看 HTTP 状态码
来源：http://hz.dashuyun.cn/gtsrpncoqu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ybcxt.top/gttacetbus.html

[R61] 磁盘占用
来源：http://hz.cqqwz.cn/gtffscihlo.html

df -h;  du -sh *
来源：http://hz.shanyushiyangkeji.top/gtjwbritmy.html

[R62] 找最占空间的文件
来源：http://hz.jinqigufen.top/gtwxnuuztk.html

du -ah . | sort -rh | head -10
来源：http://hz.andypj.xyz/gtbtjrbmnd.html

[R63] 内存与进程
来源：http://hz.yangfankeji.com/gtenmynhhw.html

free -h;  ps aux | grep nginx
来源：http://hz.zhengqikj.top/gtaqblbkhe.html

[R64] 结束进程
来源：http://hz.yj202588.top/gtyfmdgzxa.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jlsjyb.cn/gtiyqcsuvq.html

[R65] 查看端口占用
来源：http://hz.c1oappe.top/gtqsoesiar.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenzaomai.com/gtslykjfbl.html

[R66] 定时任务
来源：http://hz.316326.xyz/gtqechlnkk.html

crontab -e;  crontab -l
来源：http://hz.gogol.net.cn/gtmrapmyfa.html

[R67] 生成随机十六进制串
来源：http://hz.daxiang520.top/gtxjuyymje.html

openssl rand -hex 16
来源：http://hz.xziqi.cn/gtwewpyyia.html

[R68] 计算文件校验值
来源：http://hz.ybcxt.top/gtrcgkwjcd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.daria6918.cn/gtxigiluyh.html

[R69] 生成随机密码
来源：http://hz.chenzaomai.com/gtvyewjsse.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhiwuduotai.top/gtcondfhuj.html

[R70] 时间戳与互转
来源：http://hz.haohaochexian.top/gttyweipdp.html

date +%s;  date -d @1700000000
来源：http://hz.cqqwz.cn/gtqejdmzut.html

[R71] 日期格式化
来源：http://hz.hongshengwenyu.top/gtxxipjley.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.wangdashe.top/gtxhemexec.html

[R72] 等待端口就绪
来源：http://hz.cashguo.top/gtwmtdvagc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shuidangran.top/gtjrlwaiof.html

[R73] 分割大日志
来源：http://hz.dashuyun.cn/gtahaefxzu.html

split -l 1000 big.log part_
来源：http://hz.shuidangran.top/gtzlnmflqq.html

[R74] 批量重命名
来源：http://hz.shangyingyoupin.top/gtimenevbu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yuanzhike.top/gtcvcjcsou.html

[R75] 导出环境变量
来源：http://hz.jinyuanbaomall.cn/gtxcvspbjx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sweek.top/gtryiydgcv.html

[R76] 使用临时文件
来源：http://hz.feifeiyinyue.top/gtpnvuqtam.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gzhubu.top/gtpnvuvidw.html

[R77] 读取用户输入
来源：http://hz.zhongyouzk.top/gtlgxiynuu.html

read -rp "请输入: " ans
来源：http://hz.jinyuanbaomall.cn/gtechqhgyd.html

[R78] 交互式菜单
来源：http://hz.jiagoushi.top/gtlbtkvrgq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.quarkkingdee.top/gtnuglfsqm.html

[R79] 解析命令行选项
来源：http://hz.yvedp.cn/gtgdwhykxs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.haohaochexian.top/gtulyheggt.html

[R80] 查看脚本执行耗时
来源：http://hz.sysykeji.top/gtzpdfelgw.html

time ./run.sh
来源：http://hz.jqgfzy.top/gtihiygdun.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtvwsazbje.html

S. C / C++ 专题
来源：http://hz.xuetiantiany.cn/gthsmvkrgm.html

================================================================================
来源：http://hz.cdnleiting.top/gtodiqlluk.html

[S01] C：Hello World
来源：http://hz.gogol.net.cn/gtqlfypkus.html

#include <stdio.h>
来源：http://hz.52xcode.cn/gtqtupykee.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.haohaochexian.top/gtzdayjwng.html

[S02] C：变量与格式化输出
来源：http://hz.aibaodan.cn/gtnwuybiks.html

int a = 10; printf("%d\n", a);
来源：http://hz.ywan-chungtsiang.top/gtkfaruwkc.html

[S03] C：读入整数
来源：http://hz.c1oappe.top/gtytcfmjgp.html

int x; scanf("%d", &x);
来源：http://hz.zhoulong.xyz/gtmmcxpqpi.html

[S04] C：字符串复制
来源：http://hz.9152youxi.cn/gtkkpdzjrl.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinghuilouyu.cn/gtdodnxqvz.html

[S05] C：字符串长度
来源：http://hz.cdnleiting.top/gtejnkfdtf.html

strlen(s)
来源：http://hz.yvedp.cn/gtkdfrehlp.html

[S06] C：字符串比较
来源：http://hz.jyoumei.cn/gtebikyrxf.html

strcmp(a, b) == 0
来源：http://hz.yuanzhike.top/gtkgqfdgbj.html

[S07] C：数组遍历求和
来源：http://hz.sweek.top/gtzhmovuyx.html


<!-- 参考信息 -->