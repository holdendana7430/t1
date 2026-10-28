代发 wailian999

[Q33] 多列分组
来源：http://hz.ivvv.top/gtlgyckavx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cqqwz.cn/gtwgaysqyg.html

[Q34] 每组取第一条
来源：http://hz.havefunace.top/gtjsxbyfst.html

SELECT * FROM (
来源：http://hz.yanxiufei.cn/gtqngwjrde.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.smart0.xyz/gtycmjhlen.html

) t WHERE rn = 1;
来源：http://hz.quarkkingdee.top/gtqfougsxs.html

[Q35] 内连接
来源：http://hz.jinghuilouyu.cn/gtpkipfyzv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhijiandao.cn/gttcdpbadn.html

[Q36] 左连接
来源：http://hz.yanxiufei.cn/gtngewfutf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.quarkkingdee.top/gtaehcotav.html

[Q37] 右连接
来源：http://hz.wangdashe.top/gtwvdwilyr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.quarkkingdee.top/gtfnzsujol.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cucudq.cn/gtfjcxvxjj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xylfe.cn/gtbjwbxuto.html

[Q39] 自连接（查上下级）
来源：http://hz.chenlongwang.top/gtlwnjmqqk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shanyushiyangkeji.top/gtmatfptok.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.fengsongda.top/gttzbqeced.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.52xcode.cn/gtsszsclvs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fengsongda.top/gttpxwqxxl.html

[Q41] 多表连接
来源：http://hz.smart0.xyz/gtlkmlumvh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cqqwz.cn/gtxmmkgquy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.wangshuangyany.cn/gtazodgxjp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sysykeji.top/gtstlpwkbw.html

[Q42] 连接条件附加过滤
来源：http://hz.andypj.xyz/gtmjjxfnnl.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xinyue.icu/gtekuftqip.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hammf.cn/gthhuobcpu.html

[Q43] 标量子查询
来源：http://hz.ivvv.top/gtbiezclaf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhoulong.xyz/gtjnqphvcw.html

[Q44] IN 子查询
来源：http://hz.ybcxt.top/gtivlebhad.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.andypj.xyz/gtfvbcxzev.html

[Q45] EXISTS 判断存在
来源：http://hz.jqgufenzy.top/gtayxemqih.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shzxlz.cn/gthzovybme.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.birdmap.top/gtufljuyzo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cdnleiting.top/gttdnjsgem.html

[Q47] 与平均值比较
来源：http://hz.meibo888.top/gtuobllclz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shuidangran.top/gtxlggdrgv.html

[Q48] CTE 公用表表达式
来源：http://hz.yvedp.cn/gtrsahnfsr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cheryme.top/gtlfqbxwxi.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shanyushiyangtech.top/gtqnaoftsp.html

[Q49] 更新单行
来源：http://hz.yj202588.top/gtvkiqijio.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yangfankeji.com/gtajsoxyyy.html

[Q50] 批量更新
来源：http://hz.yj20258888.top/gtafwtbfzu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shangyingyoupin.top/gtbcjdoqjf.html

[Q51] 用子查询更新
来源：http://hz.nanxinkj.top/gthpokfahl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinghuilouyu.cn/gtqbxvtrgf.html

[Q52] 删除指定行
来源：http://hz.hnqzz.top/gthkztxuha.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jqgfzy.top/gtaaxqcovx.html

[Q53] 按条件删除
来源：http://hz.jianghu66.top/gtetoeeqie.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hammf.cn/gtfsavcqan.html

[Q54] 清空表
来源：http://hz.yueranfly.top/gtdjzigiuz.html

TRUNCATE TABLE logs;
来源：http://hz.wangdashe.top/gtwpyfcxjp.html

[Q55] 排名（并列占位）
来源：http://hz.52xcode.cn/gtphnptzir.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jqgufenzy.top/gtyearhxtb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zdqjudy.top/gtgbfnfyyp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jlsjyb.cn/gtjnpkuxvq.html

[Q57] 行号
来源：http://hz.52xcode.cn/gtoxyhnvmo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sweek.top/gtafjcfoxp.html

[Q58] 累计求和
来源：http://hz.pycfn.com/gttdxwgroi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yangfankeji.com/gtlaxldiee.html

[Q59] 分组内累计
来源：http://hz.shanyushiyangkeji.top/gtzqvtmbnt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nanxinkj.top/gthaxokcxg.html

[Q60] 取上一行 / 下一行
来源：http://hz.shanyushiyangtech.top/gtwmdzkmar.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jqgufenzy.top/gtxhlivrdx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.nanxinkj.top/gtaozqedin.html

[Q61] 移动平均
来源：http://hz.sweek.top/gtgjekfyzt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shzxlz.cn/gtqiypqnuw.html

[Q62] 分组占比
来源：http://hz.pycfn.com/gtnpsgrmek.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenjidiqi.icu/gtsruologu.html

[Q63] 开启事务
来源：http://hz.bjfxy.top/gtrdazvjzp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinqigufen.top/gteogxzfym.html

[Q64] 提交事务
来源：http://hz.quarkkingdee.top/gtrorvmirx.html

COMMIT;
来源：http://hz.9152youxi.cn/gtgkjtcrjp.html

[Q65] 回滚事务
来源：http://hz.svipenyu.cn/gtfuagyfwh.html

ROLLBACK;
来源：http://hz.smart0.xyz/gtszbfrowc.html

[Q66] 行锁查询
来源：http://hz.nwbrower.top/gtkzmgwmou.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.feifeiyinyue.top/gtltpkvptn.html

[Q67] 设置隔离级别
来源：http://hz.cqqwz.cn/gtewijdsyw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xuetiantiany.cn/gtmyrqthyp.html

[Q68] 保存点
来源：http://hz.jinyuanbaomall.cn/gtqsqikqgt.html

SAVEPOINT sp1;
来源：http://hz.tianlin.xyz/gtraieiixk.html

ROLLBACK TO sp1;
来源：http://hz.yonumen.top/gtzajifukg.html

[Q69] 查看执行计划
来源：http://hz.tanke756.top/gtqiwfdztw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tian-w.cn/gtdmnnwbzr.html

[Q70] 更新统计信息
来源：http://hz.ivvv.top/gtymjnebhd.html

ANALYZE TABLE users;
来源：http://hz.dianchejie.cn/gtndxpdohx.html

[Q71] 查看建表语句
来源：http://hz.andypj.xyz/gtzbbygrlt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.mhx1999.top/gtirolwhal.html

[Q72] 查看索引
来源：http://hz.9152youxi.cn/gtbxhmqshi.html

SHOW INDEX FROM users;
来源：http://hz.yonumen.top/gtxysdmdnw.html

[Q73] 查看表状态
来源：http://hz.yongpay.top/gttgfhvuso.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yvedp.cn/gttqfrmyxe.html

[Q74] 强制使用索引
来源：http://hz.yongpay.top/gtpfzlerwx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xingfuxueyuan.xyz/gteyeymosf.html

[Q75] 日期格式化
来源：http://hz.svipenyu.cn/gtoaeexcxq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhongyouzk.top/gtdpldyjnd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhongyouzk.top/gtqyryvrkn.html

[Q76] 按天统计
来源：http://hz.ywan-chungtsiang.top/gtjznlqekx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cdnleiting.top/gtkmiwsuhp.html

[Q77] 时间加减
来源：http://hz.yvedp.cn/gtciaaxcvl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shuidangran.top/gtpneqshed.html

[Q78] 当前时间
来源：http://hz.ivvv.top/gtvygtspla.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hongshengwenyu.top/gtcnvcunkn.html

[Q79] 字符串拼接
来源：http://hz.shanyushiyangkeji.top/gtaqyrqsnx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cucudq.cn/gtgoiqfnrx.html

[Q80] 字符串截取
来源：http://hz.jinqigufen.top/gtculvhtwx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zycfv.cn/gtwginkdjo.html

[Q81] 字符串替换
来源：http://hz.nwbrower.top/gtwosebzlf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tanke756.top/gtjkorhiao.html

[Q82] 字符长度与字节长度
来源：http://hz.hammf.cn/gtxdwmumrj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.52xcode.cn/gtgbltxttd.html

[Q83] 大小写转换
来源：http://hz.zhijiandao.cn/gtxrushzlb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cheryme.top/gtodceohmm.html

[Q84] 去除首尾空格
来源：http://hz.316326.xyz/gtfagasbzq.html

SELECT TRIM(name) FROM users;
来源：http://hz.dianchejie.cn/gthozihsmd.html

[Q85] 数值取整
来源：http://hz.zhengqikj.top/gtycooiddh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.smart0.xyz/gtcrkzqkps.html

[Q86] 读取 JSON 字段
来源：http://hz.sxryk.cn/gtfcioqydz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xylfe.cn/gtfpyqvnoq.html

[Q87] JSON 字段做条件
来源：http://hz.zhaomingkeji.xyz/gtnbhqoxoa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gogol.net.cn/gttwxyjtuw.html

[Q88] 行转列（条件聚合）
来源：http://hz.daria6918.cn/gthdjexwek.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.9152youxi.cn/gtrdtqchdt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shzxlz.cn/gtspgzyhcd.html

[Q89] 判断表是否存在
来源：http://hz.pycfn.com/gtdypjhrqo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.iojbl.cn/gtoeciremt.html

[Q90] 生成序号列
来源：http://hz.jinqigufen.top/gtrweccrkv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xziqi.cn/gtouillfnr.html

================================================================================
来源：http://hz.yonumen.top/gtclbsmazu.html

R. Bash 专题
来源：http://hz.redwolf501.top/gtiooevwww.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtdjztedby.html

[R01] shebang 与严格模式
来源：http://hz.zhixingplan.top/gtxlrglqmb.html

#!/usr/bin/env bash
来源：http://hz.gogol.net.cn/gtlxbmccpi.html

set -euo pipefail
来源：http://hz.daria6918.cn/gtapprmxyu.html

[R02] 变量赋值与使用
来源：http://hz.zhiwuduotai.top/gtuiyfpmtu.html

name="Tom"; echo "$name"
来源：http://hz.gogol.net.cn/gtjigyncim.html

[R03] 只读变量
来源：http://hz.jinqigfzy.top/gtmojxkmdl.html

readonly PI=3.14
来源：http://hz.9152youxi.cn/gtjpdibiir.html

[R04] 位置参数
来源：http://hz.yangfankeji.com/gtaglhdyda.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yvedp.cn/gtjlfeuaet.html

[R05] 参数默认值
来源：http://hz.shuidangran.top/gtadpkjwpn.html

name="${1:-default}"
来源：http://hz.cheryme.top/gtbmqgqjkm.html

[R06] 判断命令是否存在
来源：http://hz.sysykeji.top/gtbplrjvhx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yuxming.cn/gtvtgqpfet.html

[R07] if 判断文件
来源：http://hz.jinqigufen.top/gtxnclywuv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guannengcc.top/gtzfvutsdm.html

[R08] 数值比较
来源：http://hz.kuanghao11.cn/gtkucqsmuf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.52xcode.cn/gtirqhzkhx.html

[R09] 字符串比较
来源：http://hz.yj20258.top/gtlxxcrjvt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yuanzhike.top/gtsikquhec.html

[R10] 正则匹配
来源：http://hz.hnqzz.top/gtrzmkxboj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhongyouzk.top/gtrftrjhfm.html

[R11] case 多分支
来源：http://hz.ppjwa.cn/gtqoqdewcj.html

case "$1" in
来源：http://hz.yj20258888.top/gtzmbplhdm.html

start) echo "启动" ;;
来源：http://hz.yj20258.top/gtkfavwztp.html

stop)  echo "停止" ;;
来源：http://hz.xinyue.icu/gtawhcmspp.html

*)     echo "未知命令" ;;
来源：http://hz.yj202588.top/gtjszffznm.html

esac
来源：http://hz.hfpthk.cn/gtbjlzzbdk.html

[R12] for 遍历文件
来源：http://hz.meibo888.top/gtbhubbiop.html

for f in *.txt; do echo "$f"; done
来源：http://hz.guowangkeji.top/gtosxxrahf.html

[R13] for 计数循环
来源：http://hz.hnxiangtu.top/gtkjeprkfa.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.aibaodan.cn/gtptdvmffx.html

[R14] C 风格 for
来源：http://hz.xinyue.icu/gtjzujpjom.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinqigufen.top/gtivawkbtt.html

[R15] while 逐行读文件
来源：http://hz.gzhubu.top/gtwyiajmeb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ehwqpu.com/gtjnbdundv.html

[R16] until 等待条件
来源：http://hz.nanxuanxn.top/gtzpigxzrm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shanyushiyangtech.top/gtliwadhga.html

[R17] 数组定义与取值
来源：http://hz.ppjwa.cn/gthyclckjt.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hnqzz.top/gtdzoglnvd.html

[R18] 遍历数组
来源：http://hz.jinghuilouyu.cn/gtcjtwpckm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yanxiufei.cn/gtbwslhaka.html

[R19] 数组长度
来源：http://hz.pengpengdd.cyou/gtbskcizgm.html

echo "${#arr[@]}"
来源：http://hz.hnqzz.top/gtlnhvewvh.html

[R20] 关联数组（字典）
来源：http://hz.yonumen.top/gttbvtndvz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yvedp.cn/gtskgszogi.html

[R21] 字符串长度
来源：http://hz.xylfe.cn/gtximmitel.html

echo "${#s}"
来源：http://hz.zhoulong.xyz/gtgovyecsm.html

[R22] 截取子串
来源：http://hz.yj20258.top/gtlckfqzud.html

echo "${s:0:5}"
来源：http://hz.zycfv.cn/gtekkixmfo.html

[R23] 字符串替换
来源：http://hz.0kj1m.cn/gtbkhssunx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sxryk.cn/gttgauqlui.html

[R24] 大小写转换
来源：http://hz.c1oappe.top/gtoihqehnq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shanyushiyangtech.top/gtiljtixck.html

[R25] 去后缀 / 去前缀
来源：http://hz.xziqi.cn/gtoimctcsn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.guannengcc.top/gtmpqngeoy.html

[R26] 命令替换
来源：http://hz.redwolf501.top/gtcvyxxtom.html

now=$(date +%F); echo "$now"
来源：http://hz.jqgufenzy.top/gtycqthgcq.html

[R27] 算术展开
来源：http://hz.shzxlz.cn/gtmdmudima.html

echo $((1 + 2 * 3))
来源：http://hz.wangdashe.top/gtbbyusgpz.html

[R28] 浮点运算
来源：http://hz.ywan-chungtsiang.top/gtnzfgggzl.html

echo "scale=2; 10/3" | bc
来源：http://hz.hnqzz.top/gtmeonpkgl.html

[R29] 定义函数
来源：http://hz.bjfxy.top/gtyetmwlrn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guowangkeji.top/gtfowafiti.html

[R30] 函数返回状态码
来源：http://hz.cqqwz.cn/gtpafzvxbq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.aizwys.cn/gtrcgkadwy.html

[R31] 局部变量
来源：http://hz.daxiang520.top/gtkcbxzwcw.html

f() { local x=1; echo "$x"; }
来源：http://hz.hnqzz.top/gtkqdqcvhf.html

[R32] 参数个数校验
来源：http://hz.xinyue.icu/gtpvvohhax.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yvedp.cn/gtvclfynjx.html

[R33] 捕获错误并提示行号
来源：http://hz.ydzc1.top/gtosfgtkcj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.aibaodan.cn/gtaunaynvd.html

[R34] 退出时清理
来源：http://hz.gogol.net.cn/gtboknnvkr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.kuanghao11.cn/gtjbpcyzur.html

[R35] 后台执行并等待
来源：http://hz.chenzaomai.com/gtcirvcutd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yongpay.top/gtmvrqwuhe.html

[R36] 并发执行多个任务
来源：http://hz.cqqwz.cn/gtqdhmsynf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yueranfly.top/gtlcromwax.html

[R37] 把输出赋给变量
来源：http://hz.tanke756.top/gtopamtrdb.html

files=$(ls -1)
来源：http://hz.shanyushiyangtech.top/gtnapjphmv.html

[R38] 管道串联
来源：http://hz.aibaodan.cn/gtqszrqoev.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xuetiantiany.cn/gtgmvkltwm.html

[R39] 重定向标准输出与错误
来源：http://hz.jqgufenzy.top/gteecrdman.html

cmd > out.log 2>&1
来源：http://hz.zhaomingkeji.xyz/gtkdvbjibq.html

[R40] 追加写日志
来源：http://hz.meibo888.top/gtzzkpvrod.html

echo "log" >> out.log
来源：http://hz.chenzaomai.com/gtojynivix.html

[R41] 丢弃输出
来源：http://hz.wangshuangyany.cn/gtnvaqjfyd.html

cmd >/dev/null 2>&1
来源：http://hz.ydjk.org.cn/gtagzvisst.html

[R42] 输入重定向
来源：http://hz.cqqwz.cn/gtmztdqakl.html

wc -l < a.txt
来源：http://hz.jinyuanbaomall.cn/gttwviolot.html

[R43] 按名字查找文件
来源：http://hz.aibaodan.cn/gtiykmnyvu.html

find . -name "*.log" -type f
来源：http://hz.yonumen.top/gtcjmshwvn.html

[R44] 按修改时间查找
来源：http://hz.ywan-chungtsiang.top/gtlhakjfes.html

find . -mtime -7 -type f
来源：http://hz.meibo888.top/gtskzekiug.html

[R45] 批量删除
来源：http://hz.yj202588.top/gtgupamozi.html

find . -name "*.tmp" -delete
来源：http://hz.yuanzhike.top/gtvbwvlkik.html

[R46] 递归替换文件内容
来源：http://hz.yueranfly.top/gtjcmmmfny.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.fzhhl.top/gtldnbtngm.html

[R47] sed 单行替换
来源：http://hz.hywenlv.cn/gticinxzlq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinyuanbaomall.cn/gtpemjdsbg.html

[R48] awk 取指定列
来源：http://hz.ehwqpu.com/gtcaktgxld.html

awk '{print $1, $3}' a.txt
来源：http://hz.sufxvd.cn/gthffakdeo.html

[R49] awk 带条件
来源：http://hz.daxiang520.top/gtjpzsdctr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jiagoushi.top/gtrncmgfzv.html

[R50] awk 求和
来源：http://hz.yonumen.top/gtjdqeojdt.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhijiandao.cn/gtlftxidpl.html

[R51] 排序去重取前几
来源：http://hz.fengsongda.top/gtmtwkhpzj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gzhubu.top/gthxcdzjgm.html

[R52] 统计行数
来源：http://hz.ydjk.org.cn/gtnzsfyqyx.html

wc -l a.txt
来源：http://hz.jlsjyb.cn/gtguavxgei.html

[R53] 查看文件头与实时尾
来源：http://hz.bjfxy.top/gtocmknjwh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ivvv.top/gtmfpfeuci.html

[R54] 比较两个文件
来源：http://hz.dashuyun.cn/gtvnojmndd.html

diff a.txt b.txt
来源：http://hz.hysaishi.cn/gtvhslvrcd.html

[R55] 压缩与解压
来源：http://hz.haohaochexian.top/gtvkgpbyls.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhixingplan.top/gtlccvkuht.html

[R56] 远程拷贝
来源：http://hz.cqqwz.cn/gtumcpelmx.html

scp file user@host:/path/
来源：http://hz.xingfuxueyuan.xyz/gtqynalmqf.html

[R57] 远程执行命令
来源：http://hz.zhengqikj.top/gtivnhclnz.html

ssh user@host 'uptime'
来源：http://hz.haohaochexian.top/gtygptebxk.html

[R58] 下载文件
来源：http://hz.yvedp.cn/gtfydhodpv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinqigufen.top/gtqlfliquu.html

[R59] 发 POST JSON
来源：http://hz.mhx1999.top/gtggkbzmph.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shangyingyoupin.top/gthnbfkbqz.html

[R60] 只看 HTTP 状态码
来源：http://hz.vqdsnc.cn/gtyqmzosey.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhengqikj.top/gtluqovmqy.html

[R61] 磁盘占用
来源：http://hz.xinyue.icu/gtlrnaglho.html

df -h;  du -sh *
来源：http://hz.dashuyun.cn/gtveunngre.html

[R62] 找最占空间的文件
来源：http://hz.dashuyun.cn/gttzszuogh.html

du -ah . | sort -rh | head -10
来源：http://hz.zhaomingkeji.xyz/gtsbfsoswa.html

[R63] 内存与进程
来源：http://hz.hysaishi.cn/gtzbreqmzi.html

free -h;  ps aux | grep nginx
来源：http://hz.fengsongda.top/gtnbmdxkfe.html

[R64] 结束进程
来源：http://hz.daxiang520.top/gtkdzxuoin.html

kill -9 $(pgrep -f app.py)
来源：http://hz.nwbrower.top/gtabicrofq.html

[R65] 查看端口占用
来源：http://hz.ywan-chungtsiang.top/gtnggpbjza.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhiwuduotai.top/gtmxjkcjqy.html

[R66] 定时任务
来源：http://hz.ppjwa.cn/gtawdgyujy.html

crontab -e;  crontab -l
来源：http://hz.andypj.xyz/gtzdfvkkpy.html

[R67] 生成随机十六进制串
来源：http://hz.meibo888.top/gtdbdkeqms.html

openssl rand -hex 16
来源：http://hz.sufxvd.cn/gtjkipxpim.html

[R68] 计算文件校验值
来源：http://hz.xingfuxueyuan.xyz/gtkgcrtnvq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yanxiufei.cn/gtikgyzhme.html

[R69] 生成随机密码
来源：http://hz.shanyushiyangtech.top/gtjktzvwyz.html

head -c 16 /dev/urandom | base64
来源：http://hz.jlsjyb.cn/gtjximakxb.html

[R70] 时间戳与互转
来源：http://hz.xylfe.cn/gttkkxlejx.html

date +%s;  date -d @1700000000
来源：http://hz.jinqigufen.top/gtngzmfysy.html

[R71] 日期格式化
来源：http://hz.dashuyun.cn/gttizfzerr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.guowangkeji.top/gtkhdnzzto.html

[R72] 等待端口就绪
来源：http://hz.shzxlz.cn/gtbmdrowzi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhongyouzk.top/gtybbtmxnn.html

[R73] 分割大日志
来源：http://hz.haohaochexian.top/gtmrltwfqj.html

split -l 1000 big.log part_
来源：http://hz.yuxming.cn/gtmtcilsjn.html

[R74] 批量重命名
来源：http://hz.9152youxi.cn/gtvfcqalbz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ppjwa.cn/gtearpdotr.html

[R75] 导出环境变量
来源：http://hz.ppjwa.cn/gtgllpuqqn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.52xcode.cn/gtieoezhvp.html

[R76] 使用临时文件
来源：http://hz.svipenyu.cn/gtulzckmdp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.svipenyu.cn/gtabnobijq.html

[R77] 读取用户输入
来源：http://hz.gogol.net.cn/gtwlppvzau.html

read -rp "请输入: " ans
来源：http://hz.guowangkeji.top/gtcnjabjrl.html

[R78] 交互式菜单
来源：http://hz.yuanzhike.top/gtmlklwxyn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ywan-chungtsiang.top/gtlwguvuoh.html

[R79] 解析命令行选项
来源：http://hz.xuanzx.com/gtqffdafmn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jyoumei.cn/gtcrrrhlja.html

[R80] 查看脚本执行耗时
来源：http://hz.yonumen.top/gtksfnmsed.html

time ./run.sh
来源：http://hz.nanxinkj.top/gtntmvhmnu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtngehsxws.html

S. C / C++ 专题
来源：http://hz.hnxiangtu.top/gtjegzxbov.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtbyxaixub.html

[S01] C：Hello World
来源：http://hz.ydzc1.top/gtybxlsmfd.html

#include <stdio.h>
来源：http://hz.sxryk.cn/gtxcmibzth.html


<!-- 参考信息 -->