代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinyuanbaomall.cn/gthtzfyjoc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhengqikj.top/gtkezgwfis.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinqigfzy.top/gtwdjvtjiz.html

[Q41] 多表连接
来源：http://hz.gogol.net.cn/gtfpveieqa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shanyushiyangkeji.top/gtupoolasp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shuidangran.top/gtzqytnnzj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gaohongyu789.top/gtxuyamjfr.html

[Q42] 连接条件附加过滤
来源：http://hz.cucudq.cn/gtdalhqgre.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yj202588.top/gtfdxbaqhf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cucudq.cn/gtbhsdwzct.html

[Q43] 标量子查询
来源：http://hz.xuanzx.com/gtaarcwurt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.fengsongda.top/gtsceqqklf.html

[Q44] IN 子查询
来源：http://hz.jinyuanbaomall.cn/gtpsteapkq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhaomingkeji.xyz/gtxaloetpz.html

[Q45] EXISTS 判断存在
来源：http://hz.zhaomingkeji.xyz/gtxfwkydez.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhoulong.xyz/gtrpixxzju.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.daxiang520.top/gtfinotyrq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jianghu66.top/gtnblxjidy.html

[Q47] 与平均值比较
来源：http://hz.9152youxi.cn/gtbzkjzsue.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sweek.top/gtozxbefpc.html

[Q48] CTE 公用表表达式
来源：http://hz.shanyushiyangkeji.top/gtxnqtajja.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yj202588.top/gtutpidhfj.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.aibaodan.cn/gtzfiptfte.html

[Q49] 更新单行
来源：http://hz.kuanghao11.cn/gtdtewpliy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenzaomai.com/gtxvdheyfc.html

[Q50] 批量更新
来源：http://hz.yvedp.cn/gtdbfddssq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yongpay.top/gtftydgstj.html

[Q51] 用子查询更新
来源：http://hz.daxiang520.top/gtgasvomcp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.redwolf501.top/gtljjgxvfz.html

[Q52] 删除指定行
来源：http://hz.xuetiantiany.cn/gtbszvdvxd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gaohongyu789.top/gtuzenxhah.html

[Q53] 按条件删除
来源：http://hz.guowangkeji.top/gtvdqvikbr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.vqdsnc.cn/gtavegrkgm.html

[Q54] 清空表
来源：http://hz.jinqigufen.top/gtlohiydok.html

TRUNCATE TABLE logs;
来源：http://hz.ydjk.org.cn/gtzqhiwvjw.html

[Q55] 排名（并列占位）
来源：http://hz.nwbrower.top/gtxcllcqru.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.mhx1999.top/gtqhabqfzq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yuanzhike.top/gteglopplm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj20258.top/gtanfzbret.html

[Q57] 行号
来源：http://hz.birdmap.top/gtzplyqyes.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xuetiantiany.cn/gttsrklxwz.html

[Q58] 累计求和
来源：http://hz.sufxvd.cn/gtikaptnpt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.fzhhl.top/gtphdjtrwl.html

[Q59] 分组内累计
来源：http://hz.jiagoushi.top/gtcwjioylb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.svipenyu.cn/gtktyakdvg.html

[Q60] 取上一行 / 下一行
来源：http://hz.jqgufenzy.top/gtsuugeizm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ydjk.org.cn/gtszvzqefl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cdnleiting.top/gtlvyvgcny.html

[Q61] 移动平均
来源：http://hz.andypj.xyz/gteenrbdlz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yvedp.cn/gtytsnensx.html

[Q62] 分组占比
来源：http://hz.dashuyun.cn/gtctsxczgw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yuxming.cn/gtabziokym.html

[Q63] 开启事务
来源：http://hz.xuetiantiany.cn/gtnvjrzezc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gaohongyu789.top/gtebhnoupt.html

[Q64] 提交事务
来源：http://hz.cheryme.top/gtclivifwq.html

COMMIT;
来源：http://hz.iojbl.cn/gtwfgryoij.html

[Q65] 回滚事务
来源：http://hz.dianchejie.cn/gtjbgdjlbq.html

ROLLBACK;
来源：http://hz.hammf.cn/gtagaaoobr.html

[Q66] 行锁查询
来源：http://hz.jlsjyb.cn/gthfzynvwo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tanke756.top/gtauvmxyfe.html

[Q67] 设置隔离级别
来源：http://hz.zhiwuduotai.top/gtdhtufmym.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cqqwz.cn/gtsjbcwgds.html

[Q68] 保存点
来源：http://hz.zhixingplan.top/gtcijacsmf.html

SAVEPOINT sp1;
来源：http://hz.chenjidiqi.icu/gtpmqwgrid.html

ROLLBACK TO sp1;
来源：http://hz.gzhubu.top/gtblcaxxzj.html

[Q69] 查看执行计划
来源：http://hz.zdqjudy.top/gtelycskhr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hammf.cn/gtvbegxbfa.html

[Q70] 更新统计信息
来源：http://hz.xziqi.cn/gttsjmrxbo.html

ANALYZE TABLE users;
来源：http://hz.nanxuanxn.top/gtvjwrswpm.html

[Q71] 查看建表语句
来源：http://hz.feifeiyinyue.top/gtboerhlsw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.52xcode.cn/gtxhxeyvws.html

[Q72] 查看索引
来源：http://hz.hnqzz.top/gtkwwrzflt.html

SHOW INDEX FROM users;
来源：http://hz.shanyushiyangtech.top/gtzttpuaoq.html

[Q73] 查看表状态
来源：http://hz.zhoulong.xyz/gtorgrqqvq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.daxiang520.top/gtpiwwiqut.html

[Q74] 强制使用索引
来源：http://hz.quarkkingdee.top/gtuqixxsyt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.meibo888.top/gtaumzmhgx.html

[Q75] 日期格式化
来源：http://hz.yongpay.top/gtfuekyxvw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jianghu66.top/gtlcunaplh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.meibo888.top/gtgsotuxga.html

[Q76] 按天统计
来源：http://hz.birdmap.top/gtkxsnubct.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hfpthk.cn/gtizaqhbbr.html

[Q77] 时间加减
来源：http://hz.daxiang520.top/gtspshhtqs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.daria6918.cn/gtcfqexool.html

[Q78] 当前时间
来源：http://hz.pengpengdd.cyou/gtzfbyljmp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hnqzz.top/gtbtcupmox.html

[Q79] 字符串拼接
来源：http://hz.52xcode.cn/gtlhvbeqwv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hysaishi.cn/gtvsqjvypj.html

[Q80] 字符串截取
来源：http://hz.guannengcc.top/gtzeqzuhwo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenlongwang.top/gtbrpnbrid.html

[Q81] 字符串替换
来源：http://hz.sysykeji.top/gtiswugmdl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenzaomai.com/gtvrnrhvgd.html

[Q82] 字符长度与字节长度
来源：http://hz.chenlongwang.top/gtipdvkzfx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ybcxt.top/gtjuqaxqsf.html

[Q83] 大小写转换
来源：http://hz.316326.xyz/gtvyegywow.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cucudq.cn/gtomcnukzp.html

[Q84] 去除首尾空格
来源：http://hz.yj20258888.top/gtvctipyyb.html

SELECT TRIM(name) FROM users;
来源：http://hz.hysaishi.cn/gtzseczsid.html

[Q85] 数值取整
来源：http://hz.jiagoushi.top/gtjarlnotw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tian-w.cn/gtlmiffyoc.html

[Q86] 读取 JSON 字段
来源：http://hz.0kj1m.cn/gtkygjbuzv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.daxiang520.top/gtlfsdfzmn.html

[Q87] JSON 字段做条件
来源：http://hz.jqgfzy.top/gtsjjyquro.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gotoacloud.top/gtiwuuevmo.html

[Q88] 行转列（条件聚合）
来源：http://hz.52xcode.cn/gtpijdrthw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.aibaodan.cn/gtcjgattqw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shangyingyoupin.top/gtbhfekwtc.html

[Q89] 判断表是否存在
来源：http://hz.fengsongda.top/gtymwrfrcu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hongshengwenyu.top/gtozerirfk.html

[Q90] 生成序号列
来源：http://hz.dianchejie.cn/gtjqlpuqxo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinqigfzy.top/gtwfaimehn.html

================================================================================
来源：http://hz.tianlin.xyz/gthwbriyzw.html

R. Bash 专题
来源：http://hz.vqdsnc.cn/gtynofvrxc.html

================================================================================
来源：http://hz.9152youxi.cn/gtzivysrrr.html

[R01] shebang 与严格模式
来源：http://hz.jinghuilouyu.cn/gtmjnolarb.html

#!/usr/bin/env bash
来源：http://hz.yj202588.top/gtyztlkghk.html

set -euo pipefail
来源：http://hz.birdmap.top/gtdxtnvhhq.html

[R02] 变量赋值与使用
来源：http://hz.gogol.net.cn/gtfcsdninz.html

name="Tom"; echo "$name"
来源：http://hz.hysaishi.cn/gtigrwszhb.html

[R03] 只读变量
来源：http://hz.yj20258888.top/gtuozlwfay.html

readonly PI=3.14
来源：http://hz.daxiang520.top/gtbultkdfd.html

[R04] 位置参数
来源：http://hz.zhaomingkeji.xyz/gtfjtgxdln.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj20258888.top/gttbxgwfzf.html

[R05] 参数默认值
来源：http://hz.zycfv.cn/gtjblqksxl.html

name="${1:-default}"
来源：http://hz.zdqjudy.top/gtphduvihv.html

[R06] 判断命令是否存在
来源：http://hz.iojbl.cn/gtbdvueygd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sxryk.cn/gtfemvkojl.html

[R07] if 判断文件
来源：http://hz.wangdashe.top/gtibcbymuv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shangyingyoupin.top/gtqqougddl.html

[R08] 数值比较
来源：http://hz.shanyushiyangtech.top/gtcfqlsklh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ehwqpu.com/gtfqiourhg.html

[R09] 字符串比较
来源：http://hz.yuxming.cn/gtsyoicfgn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.redwolf501.top/gtukelgqwr.html

[R10] 正则匹配
来源：http://hz.shzxlz.cn/gtyyrtqheg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.kuanghao11.cn/gtfsuhkbok.html

[R11] case 多分支
来源：http://hz.redwolf501.top/gtktdgznzx.html

case "$1" in
来源：http://hz.gotoacloud.top/gtjtzkdwru.html

start) echo "启动" ;;
来源：http://hz.bjfxy.top/gtnnifvhjl.html

stop)  echo "停止" ;;
来源：http://hz.aibaodan.cn/gtswykzyfa.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangkeji.top/gttedeammn.html

esac
来源：http://hz.svipenyu.cn/gtmvqudwob.html

[R12] for 遍历文件
来源：http://hz.yuanzhike.top/gtqivnooed.html

for f in *.txt; do echo "$f"; done
来源：http://hz.birdmap.top/gtjxwgfcfi.html

[R13] for 计数循环
来源：http://hz.chenjidiqi.icu/gtrowkwkqq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.c1oappe.top/gtbskksgfr.html

[R14] C 风格 for
来源：http://hz.meibo888.top/gtbsqxmmjo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cucudq.cn/gtzcicpbzu.html

[R15] while 逐行读文件
来源：http://hz.nanxuanxn.top/gttsxevlwb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.9152youxi.cn/gtufscjxqb.html

[R16] until 等待条件
来源：http://hz.aizwys.cn/gtvowbdbcl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jqgufenzy.top/gtgzqlehqr.html

[R17] 数组定义与取值
来源：http://hz.xuanzx.com/gtvmbazbji.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ydjk.org.cn/gttajemckr.html

[R18] 遍历数组
来源：http://hz.feifeiyinyue.top/gtilwkkbja.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zycfv.cn/gtqdzuzqlu.html

[R19] 数组长度
来源：http://hz.xuetiantiany.cn/gtvadhmbad.html

echo "${#arr[@]}"
来源：http://hz.shanyushiyangtech.top/gtxjotqatc.html

[R20] 关联数组（字典）
来源：http://hz.chenjidiqi.icu/gtpawsuare.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sysykeji.top/gtrkrzxtbd.html

[R21] 字符串长度
来源：http://hz.tian-w.cn/gtbbjicwry.html

echo "${#s}"
来源：http://hz.jlsjyb.cn/gttlzkmpdt.html

[R22] 截取子串
来源：http://hz.zhiwuduotai.top/gtmaaxmruf.html

echo "${s:0:5}"
来源：http://hz.hnqzz.top/gtijjtbwze.html

[R23] 字符串替换
来源：http://hz.ybcxt.top/gtktyeuvxq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yuxming.cn/gtcwrfgeua.html

[R24] 大小写转换
来源：http://hz.tianlin.xyz/gtgumyjzze.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.c1oappe.top/gtelevwztg.html

[R25] 去后缀 / 去前缀
来源：http://hz.aibaodan.cn/gtnjppmyop.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yueranfly.top/gtgoyvsksg.html

[R26] 命令替换
来源：http://hz.meibo888.top/gttdeciips.html

now=$(date +%F); echo "$now"
来源：http://hz.ywan-chungtsiang.top/gtohjbnbmb.html

[R27] 算术展开
来源：http://hz.jinqigufen.top/gtfvlslygn.html

echo $((1 + 2 * 3))
来源：http://hz.haohaochexian.top/gtnknctocv.html

[R28] 浮点运算
来源：http://hz.jlsjyb.cn/gtqslssams.html

echo "scale=2; 10/3" | bc
来源：http://hz.ywan-chungtsiang.top/gtmundqfez.html

[R29] 定义函数
来源：http://hz.daxiang520.top/gtxulsnker.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.wangshuangyany.cn/gteyrpqbto.html

[R30] 函数返回状态码
来源：http://hz.aizwys.cn/gtxudxnjmg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gaohongyu789.top/gtygpqyysd.html

[R31] 局部变量
来源：http://hz.hnxiangtu.top/gtksnihrie.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhengqikj.top/gtpdzzmfyc.html

[R32] 参数个数校验
来源：http://hz.52xcode.cn/gtqfjwsqiq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ywan-chungtsiang.top/gtmoqadcbk.html

[R33] 捕获错误并提示行号
来源：http://hz.feifeiyinyue.top/gtlosceiks.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.daria6918.cn/gtuvingszy.html

[R34] 退出时清理
来源：http://hz.zhaomingkeji.xyz/gtwebpfldj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigufen.top/gtkzctpofn.html

[R35] 后台执行并等待
来源：http://hz.shangyingyoupin.top/gtddimsfsf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.fzhhl.top/gtegcnftoi.html

[R36] 并发执行多个任务
来源：http://hz.dashuyun.cn/gtjtppsgjp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.aibaodan.cn/gtidrewgcj.html

[R37] 把输出赋给变量
来源：http://hz.mhx1999.top/gtqujsynwm.html

files=$(ls -1)
来源：http://hz.ybcxt.top/gtnrlhqzcy.html

[R38] 管道串联
来源：http://hz.hongshengwenyu.top/gtycahnefe.html

cat a.txt | grep -i error | wc -l
来源：http://hz.vqdsnc.cn/gtlgxfrxxq.html

[R39] 重定向标准输出与错误
来源：http://hz.zhengqikj.top/gttlojawxu.html

cmd > out.log 2>&1
来源：http://hz.bjfxy.top/gtlbxzkgdr.html

[R40] 追加写日志
来源：http://hz.jyoumei.cn/gtzgdcatbm.html

echo "log" >> out.log
来源：http://hz.zhijiandao.cn/gtzuxmicxw.html

[R41] 丢弃输出
来源：http://hz.316326.xyz/gtjinnpxul.html

cmd >/dev/null 2>&1
来源：http://hz.aibaodan.cn/gtewpckqdt.html

[R42] 输入重定向
来源：http://hz.nwbrower.top/gtwrfebluo.html

wc -l < a.txt
来源：http://hz.gzhubu.top/gtokzqakpw.html

[R43] 按名字查找文件
来源：http://hz.yj20258.top/gturshdbxf.html

find . -name "*.log" -type f
来源：http://hz.ivvv.top/gtvsecxanr.html

[R44] 按修改时间查找
来源：http://hz.jinqigfzy.top/gtmrkscgyn.html

find . -mtime -7 -type f
来源：http://hz.birdmap.top/gtfyczkiwd.html

[R45] 批量删除
来源：http://hz.snrcjt.cn/gtycbxuasb.html

find . -name "*.tmp" -delete
来源：http://hz.gzhubu.top/gtnebdauzq.html

[R46] 递归替换文件内容
来源：http://hz.shanyushiyangkeji.top/gtmvgrgfcd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yueranfly.top/gtdbhxjtpn.html

[R47] sed 单行替换
来源：http://hz.xingfuxueyuan.xyz/gtzqzpzgtp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sweek.top/gthluycvck.html

[R48] awk 取指定列
来源：http://hz.guannengcc.top/gtogddwylf.html

awk '{print $1, $3}' a.txt
来源：http://hz.daria6918.cn/gtkhfulepe.html

[R49] awk 带条件
来源：http://hz.yj20258.top/gtfwzcsyxx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xuanzx.com/gtstehvssm.html

[R50] awk 求和
来源：http://hz.gaohongyu789.top/gtrbgmvhcf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.tian-w.cn/gtwccdgakr.html

[R51] 排序去重取前几
来源：http://hz.0kj1m.cn/gtfgkyljxw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydjk.org.cn/gtpnybetkj.html

[R52] 统计行数
来源：http://hz.zycfv.cn/gtezhoqvtj.html

wc -l a.txt
来源：http://hz.jinqigufen.top/gtjpdnnmnc.html

[R53] 查看文件头与实时尾
来源：http://hz.sufxvd.cn/gtdrltnmui.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dashuyun.cn/gtyknqxzbw.html

[R54] 比较两个文件
来源：http://hz.0kj1m.cn/gtewkpqjfb.html

diff a.txt b.txt
来源：http://hz.aizwys.cn/gtfvglxobn.html

[R55] 压缩与解压
来源：http://hz.dianchejie.cn/gtjlxleeus.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dashuyun.cn/gtqsswcyuu.html

[R56] 远程拷贝
来源：http://hz.yuxming.cn/gtkjqrsdvp.html

scp file user@host:/path/
来源：http://hz.pycfn.com/gtrrlloyta.html

[R57] 远程执行命令
来源：http://hz.redwolf501.top/gtsvngohul.html

ssh user@host 'uptime'
来源：http://hz.zhixingplan.top/gtrgyfrkdu.html

[R58] 下载文件
来源：http://hz.9152youxi.cn/gtkzhthqkf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tian-w.cn/gtljvqrkgq.html

[R59] 发 POST JSON
来源：http://hz.daxiang520.top/gtbxcibabs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.tianlin.xyz/gtweonehhb.html

[R60] 只看 HTTP 状态码
来源：http://hz.hnxiangtu.top/gtlpfcwrnl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jyoumei.cn/gtnlimjnqr.html

[R61] 磁盘占用
来源：http://hz.jinyuanbaomall.cn/gtynvrcqqd.html

df -h;  du -sh *
来源：http://hz.vqdsnc.cn/gtqktyvffg.html

[R62] 找最占空间的文件
来源：http://hz.sxryk.cn/gtpwnxrutb.html

du -ah . | sort -rh | head -10
来源：http://hz.yj20258888.top/gtnpaqbrxd.html

[R63] 内存与进程
来源：http://hz.gogol.net.cn/gtgznvahgu.html

free -h;  ps aux | grep nginx
来源：http://hz.cashguo.top/gthfswyvnj.html

[R64] 结束进程
来源：http://hz.jianghu66.top/gtzlzdgtcv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xziqi.cn/gtwguolkat.html

[R65] 查看端口占用
来源：http://hz.mhx1999.top/gtqixivklj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ywan-chungtsiang.top/gtqwxccwjp.html

[R66] 定时任务
来源：http://hz.zhixingplan.top/gtpfcvlacl.html

crontab -e;  crontab -l
来源：http://hz.hammf.cn/gtypglyobo.html

[R67] 生成随机十六进制串
来源：http://hz.yj202588.top/gtknccgolv.html

openssl rand -hex 16
来源：http://hz.yueranfly.top/gteueemino.html

[R68] 计算文件校验值
来源：http://hz.tianlin.xyz/gtcathvrzd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangtech.top/gtxxyrllkt.html

[R69] 生成随机密码
来源：http://hz.meibo888.top/gtwdxwxlyc.html

head -c 16 /dev/urandom | base64
来源：http://hz.0kj1m.cn/gtuefjkocv.html

[R70] 时间戳与互转
来源：http://hz.ywan-chungtsiang.top/gtqevucnhu.html

date +%s;  date -d @1700000000
来源：http://hz.ppjwa.cn/gtnlcgzrpq.html

[R71] 日期格式化
来源：http://hz.yj20258888.top/gttewrwlek.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinqigufen.top/gtogglkgbb.html

[R72] 等待端口就绪
来源：http://hz.xuanzx.com/gtgowjktvt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.0kj1m.cn/gtqergefrz.html

[R73] 分割大日志
来源：http://hz.jinqigufen.top/gtkmgtbarv.html

split -l 1000 big.log part_
来源：http://hz.aizwys.cn/gtozbjrysd.html

[R74] 批量重命名
来源：http://hz.xuetiantiany.cn/gtauuwaboy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jiagoushi.top/gtqqzbbbnd.html

[R75] 导出环境变量
来源：http://hz.c1oappe.top/gtenpxalqc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.aibaodan.cn/gtphhlzprp.html

[R76] 使用临时文件
来源：http://hz.cheryme.top/gtgpnmgsqf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zdqjudy.top/gtsgjpfxvg.html

[R77] 读取用户输入
来源：http://hz.shzxlz.cn/gtofeyofuu.html

read -rp "请输入: " ans
来源：http://hz.aibaodan.cn/gtqdldqfqu.html

[R78] 交互式菜单
来源：http://hz.yvedp.cn/gtkhrkrbmf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zycfv.cn/gtbxonhxwp.html

[R79] 解析命令行选项
来源：http://hz.aizwys.cn/gtiuqefjwh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.fzhhl.top/gtlmmqczhh.html

[R80] 查看脚本执行耗时
来源：http://hz.jinghuilouyu.cn/gtmqaccyeo.html

time ./run.sh
来源：http://hz.tanke756.top/gtmlbzezad.html

================================================================================
来源：http://hz.ehwqpu.com/gtycltxuty.html

S. C / C++ 专题
来源：http://hz.zhiwuduotai.top/gthiumbgvs.html

================================================================================
来源：http://hz.gogol.net.cn/gtdrqrgsbm.html

[S01] C：Hello World
来源：http://hz.tanke756.top/gtcvhczezo.html

#include <stdio.h>
来源：http://hz.9152youxi.cn/gtcmzitfzk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hammf.cn/gtlhvunnko.html

[S02] C：变量与格式化输出
来源：http://hz.jyoumei.cn/gtpfacxhri.html

int a = 10; printf("%d\n", a);
来源：http://hz.smart0.xyz/gtyyznulma.html

[S03] C：读入整数
来源：http://hz.nanxuanxn.top/gtzvbwjxhd.html

int x; scanf("%d", &x);
来源：http://hz.jinghuilouyu.cn/gtjghgswca.html

[S04] C：字符串复制
来源：http://hz.yj202588.top/gtagqaimyt.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhoulong.xyz/gtajjcfyzt.html

[S05] C：字符串长度
来源：http://hz.guowangkeji.top/gtfybgfdwt.html

strlen(s)
来源：http://hz.sxryk.cn/gtkhzlodjj.html

[S06] C：字符串比较
来源：http://hz.jinyuanbaomall.cn/gtdmgfnfov.html

strcmp(a, b) == 0
来源：http://hz.vqdsnc.cn/gtzfwzkgzz.html

[S07] C：数组遍历求和
来源：http://hz.pycfn.com/gtjrwiqlxw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.fengsongda.top/gtlgyiwpcj.html

[S08] C：动态内存分配与释放
来源：http://hz.guowangkeji.top/gtxxwnzbds.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinyuanbaomall.cn/gtzldpwmoi.html

[S09] C：结构体定义与初始化
来源：http://hz.pycfn.com/gtqzekyorf.html


<!-- 参考信息 -->