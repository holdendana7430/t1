代发 wailian999

[Q33] 多列分组
来源：http://hz.zhengqikj.top/gtqgodxwgo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.quarkkingdee.top/gtrvbxjbdt.html

[Q34] 每组取第一条
来源：http://hz.hnxiangtu.top/gtkqofgake.html

SELECT * FROM (
来源：http://hz.xziqi.cn/gtfuvcufev.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ydjk.org.cn/gtzsjwckbh.html

) t WHERE rn = 1;
来源：http://hz.shangyingyoupin.top/gtyopoosnm.html

[Q35] 内连接
来源：http://hz.sweek.top/gthmiqsuxq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.havefunace.top/gtplygkpic.html

[Q36] 左连接
来源：http://hz.0kj1m.cn/gtupyxshme.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hammf.cn/gtvcusejjh.html

[Q37] 右连接
来源：http://hz.havefunace.top/gtcahpubgi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ppjwa.cn/gtjcalwtcu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.aibaodan.cn/gtyoejlanx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhongyouzk.top/gtuoqrspzh.html

[Q39] 自连接（查上下级）
来源：http://hz.nwbrower.top/gtcukyxoth.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zycfv.cn/gtpgcateet.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.wangdashe.top/gtnfkekgkk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.52xcode.cn/gtrdvknrex.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yongpay.top/gtgyiuidhf.html

[Q41] 多表连接
来源：http://hz.pengpengdd.cyou/gttoorupex.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hysaishi.cn/gtnophhbyr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.aibaodan.cn/gtonprkfnr.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.kuanghao11.cn/gtzriruchi.html

[Q42] 连接条件附加过滤
来源：http://hz.gaohongyu789.top/gtzaodwfho.html

SELECT u.name, o.amount FROM users u
来源：http://hz.daxiang520.top/gtctskovgl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.52xcode.cn/gtucvisdcx.html

[Q43] 标量子查询
来源：http://hz.hywenlv.cn/gtjiapuknm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhaomingkeji.xyz/gtphiujjet.html

[Q44] IN 子查询
来源：http://hz.jqgufenzy.top/gtwrdozfbo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yongpay.top/gtkqcjrlwc.html

[Q45] EXISTS 判断存在
来源：http://hz.pycfn.com/gtjpgprejs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinghuilouyu.cn/gtxfbwecjx.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sweek.top/gtdbnmdoqu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hfpthk.cn/gteafthmnu.html

[Q47] 与平均值比较
来源：http://hz.iojbl.cn/gtisecjxne.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinqigufen.top/gtyqfdrirc.html

[Q48] CTE 公用表表达式
来源：http://hz.hfpthk.cn/gtemfphusp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xuetiantiany.cn/gtizixyxwa.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.guowangkeji.top/gtdkicrwrs.html

[Q49] 更新单行
来源：http://hz.yanxiufei.cn/gtqiiygsfm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.tian-w.cn/gthncbjfrf.html

[Q50] 批量更新
来源：http://hz.aibaodan.cn/gtgajbqola.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jqgufenzy.top/gtjymqyeet.html

[Q51] 用子查询更新
来源：http://hz.nanxuanxn.top/gtahaulqqu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.snrcjt.cn/gtoedgmxli.html

[Q52] 删除指定行
来源：http://hz.xuanzx.com/gtazcjdxgd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ppjwa.cn/gtzmfjrdyg.html

[Q53] 按条件删除
来源：http://hz.chenjidiqi.icu/gtbgzzccrg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yuanzhike.top/gtgctblarr.html

[Q54] 清空表
来源：http://hz.gaohongyu789.top/gtznnkuiap.html

TRUNCATE TABLE logs;
来源：http://hz.jyoumei.cn/gtqqfbdtbh.html

[Q55] 排名（并列占位）
来源：http://hz.bjfxy.top/gtndqjijmw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.52xcode.cn/gtwpmxftnj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.meibo888.top/gtejfzsfrk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hywenlv.cn/gtogtqhxtk.html

[Q57] 行号
来源：http://hz.hysaishi.cn/gtdygxwvic.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.daria6918.cn/gtpvizsljo.html

[Q58] 累计求和
来源：http://hz.cdnleiting.top/gtjgiodudo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.c1oappe.top/gtynpdcrcv.html

[Q59] 分组内累计
来源：http://hz.shanyushiyangkeji.top/gtpvbglwnv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtmxhxbqkj.html

[Q60] 取上一行 / 下一行
来源：http://hz.jqgufenzy.top/gtzaiedtyb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.havefunace.top/gtqujzqhpb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.mhx1999.top/gtcugognsl.html

[Q61] 移动平均
来源：http://hz.quarkkingdee.top/gtxjobommw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.nwbrower.top/gtvimeplbb.html

[Q62] 分组占比
来源：http://hz.jinqigfzy.top/gtpjtbgprc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cqqwz.cn/gtxtcijyng.html

[Q63] 开启事务
来源：http://hz.jianghu66.top/gtlstyscoh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxinkj.top/gtwxknnffd.html

[Q64] 提交事务
来源：http://hz.yvedp.cn/gttmcbundi.html

COMMIT;
来源：http://hz.jinyuanbaomall.cn/gtzbaselfk.html

[Q65] 回滚事务
来源：http://hz.dianchejie.cn/gtjocogpsq.html

ROLLBACK;
来源：http://hz.hongshengwenyu.top/gttimjjthc.html

[Q66] 行锁查询
来源：http://hz.svipenyu.cn/gtroatwovw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sufxvd.cn/gtabrmvtgx.html

[Q67] 设置隔离级别
来源：http://hz.gogol.net.cn/gtjjsiicme.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.pycfn.com/gtwszntyyi.html

[Q68] 保存点
来源：http://hz.iojbl.cn/gtlaebsltb.html

SAVEPOINT sp1;
来源：http://hz.zhaomingkeji.xyz/gtwhyboqsx.html

ROLLBACK TO sp1;
来源：http://hz.hysaishi.cn/gtlpeviecr.html

[Q69] 查看执行计划
来源：http://hz.yj20258.top/gtndigfgma.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yueranfly.top/gtetddvjzt.html

[Q70] 更新统计信息
来源：http://hz.smart0.xyz/gtdudrckbb.html

ANALYZE TABLE users;
来源：http://hz.pengpengdd.cyou/gtdrusicxi.html

[Q71] 查看建表语句
来源：http://hz.cdnleiting.top/gtvwerdebh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.wangshuangyany.cn/gtkhwshdad.html

[Q72] 查看索引
来源：http://hz.jlsjyb.cn/gtycpkbdpn.html

SHOW INDEX FROM users;
来源：http://hz.ppjwa.cn/gtxcbywkno.html

[Q73] 查看表状态
来源：http://hz.xingfuxueyuan.xyz/gtcrppiqmn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xinyue.icu/gtvfujeknl.html

[Q74] 强制使用索引
来源：http://hz.sufxvd.cn/gtjypgdznk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hnqzz.top/gtbyivdoov.html

[Q75] 日期格式化
来源：http://hz.havefunace.top/gtdflfkelu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zycfv.cn/gtrfyhwgfp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ywan-chungtsiang.top/gtcvgclhhy.html

[Q76] 按天统计
来源：http://hz.jinqigufen.top/gthbhethyu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.wangdashe.top/gtcqwfseit.html

[Q77] 时间加减
来源：http://hz.cucudq.cn/gtxwxobeps.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.316326.xyz/gtumhvzgls.html

[Q78] 当前时间
来源：http://hz.snrcjt.cn/gtplwdykxg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shangyingyoupin.top/gthwjixayi.html

[Q79] 字符串拼接
来源：http://hz.yj202588.top/gthsghhnfp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zycfv.cn/gtolenmurf.html

[Q80] 字符串截取
来源：http://hz.guannengcc.top/gtkodlfxkl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yangfankeji.com/gtglwlylug.html

[Q81] 字符串替换
来源：http://hz.ppjwa.cn/gtxjndenie.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ywan-chungtsiang.top/gtjhatkxbs.html

[Q82] 字符长度与字节长度
来源：http://hz.yueranfly.top/gtlgjduxaa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shuidangran.top/gtrbufnagf.html

[Q83] 大小写转换
来源：http://hz.hongshengwenyu.top/gtjusihcbb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yvedp.cn/gtaoexdngu.html

[Q84] 去除首尾空格
来源：http://hz.zhiwuduotai.top/gtztxdqamq.html

SELECT TRIM(name) FROM users;
来源：http://hz.52xcode.cn/gtqebvhtra.html

[Q85] 数值取整
来源：http://hz.0kj1m.cn/gttpsrmrwz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jqgufenzy.top/gtqqohsytl.html

[Q86] 读取 JSON 字段
来源：http://hz.fzhhl.top/gtcrmhsxch.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shanyushiyangtech.top/gtawssrunv.html

[Q87] JSON 字段做条件
来源：http://hz.xylfe.cn/gttlygmpyc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.haohaochexian.top/gtamvvcuzn.html

[Q88] 行转列（条件聚合）
来源：http://hz.smart0.xyz/gtsbtceour.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jianghu66.top/gtjmhjyehd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hfpthk.cn/gtdbmrfsnz.html

[Q89] 判断表是否存在
来源：http://hz.aizwys.cn/gtglyuuhcl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gogol.net.cn/gtcwgpskpt.html

[Q90] 生成序号列
来源：http://hz.nanxinkj.top/gtqkbhajel.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.guannengcc.top/gtmdftoazb.html

================================================================================
来源：http://hz.dianchejie.cn/gtdbbixkzr.html

R. Bash 专题
来源：http://hz.shuidangran.top/gtolqvmgzl.html

================================================================================
来源：http://hz.guannengcc.top/gtldypwweb.html

[R01] shebang 与严格模式
来源：http://hz.zhengqikj.top/gthkihafev.html

#!/usr/bin/env bash
来源：http://hz.sxryk.cn/gtvwgaxled.html

set -euo pipefail
来源：http://hz.wangshuangyany.cn/gtwzsyndhz.html

[R02] 变量赋值与使用
来源：http://hz.dashuyun.cn/gtxjhepfad.html

name="Tom"; echo "$name"
来源：http://hz.tanke756.top/gthpgxwzoh.html

[R03] 只读变量
来源：http://hz.yuanzhike.top/gtskiorcch.html

readonly PI=3.14
来源：http://hz.smart0.xyz/gtsnjjwpvj.html

[R04] 位置参数
来源：http://hz.shanyushiyangtech.top/gtfqlcltxs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.redwolf501.top/gttiqcxuna.html

[R05] 参数默认值
来源：http://hz.ivvv.top/gtztgohkds.html

name="${1:-default}"
来源：http://hz.cqqwz.cn/gtndmlgyji.html

[R06] 判断命令是否存在
来源：http://hz.sxryk.cn/gtbhjczojt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yuanzhike.top/gtgltsiyaw.html

[R07] if 判断文件
来源：http://hz.cdnleiting.top/gtnqutcfrj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.aizwys.cn/gtulowjnlu.html

[R08] 数值比较
来源：http://hz.nanxuanxn.top/gtovqgassq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ydzc1.top/gticmkpmpk.html

[R09] 字符串比较
来源：http://hz.meibo888.top/gtprzbnyps.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shanyushiyangkeji.top/gtosgkxxpk.html

[R10] 正则匹配
来源：http://hz.cheryme.top/gtvzjteqee.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhengqikj.top/gtvpgjupfm.html

[R11] case 多分支
来源：http://hz.chenjidiqi.icu/gtefmzqmab.html

case "$1" in
来源：http://hz.wangshuangyany.cn/gtxfcvtmkp.html

start) echo "启动" ;;
来源：http://hz.daria6918.cn/gtwxsgtfjp.html

stop)  echo "停止" ;;
来源：http://hz.yj20258888.top/gtuccjbnvn.html

*)     echo "未知命令" ;;
来源：http://hz.jinghuilouyu.cn/gtbzencnzt.html

esac
来源：http://hz.tanke756.top/gtjmiytmxz.html

[R12] for 遍历文件
来源：http://hz.gotoacloud.top/gtbngztbqo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.daria6918.cn/gtyrugkzss.html

[R13] for 计数循环
来源：http://hz.yvedp.cn/gtfowptswt.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yvedp.cn/gthopzjzkq.html

[R14] C 风格 for
来源：http://hz.jyoumei.cn/gtuiawbxnj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.haohaochexian.top/gtusjkylng.html

[R15] while 逐行读文件
来源：http://hz.xinyue.icu/gtymntudie.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jqgufenzy.top/gtiooxeeba.html

[R16] until 等待条件
来源：http://hz.bjfxy.top/gtfwkiymow.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.52xcode.cn/gtwyzxhtov.html

[R17] 数组定义与取值
来源：http://hz.vqdsnc.cn/gtcgugmjak.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cdnleiting.top/gtlclzpocd.html

[R18] 遍历数组
来源：http://hz.ppjwa.cn/gtnswgnrhw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangkeji.top/gtakvequdz.html

[R19] 数组长度
来源：http://hz.jianghu66.top/gtxekxvmeh.html

echo "${#arr[@]}"
来源：http://hz.bjfxy.top/gtezbgoqhr.html

[R20] 关联数组（字典）
来源：http://hz.xuanzx.com/gthkctxvkw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hysaishi.cn/gtqyyagpkw.html

[R21] 字符串长度
来源：http://hz.zhijiandao.cn/gtekxfpsfi.html

echo "${#s}"
来源：http://hz.ywan-chungtsiang.top/gtigtzozvi.html

[R22] 截取子串
来源：http://hz.kuanghao11.cn/gtzzlzxtvm.html

echo "${s:0:5}"
来源：http://hz.jinqigufen.top/gtdlnhoplp.html

[R23] 字符串替换
来源：http://hz.hysaishi.cn/gtdonierhe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.iojbl.cn/gtvmppress.html

[R24] 大小写转换
来源：http://hz.c1oappe.top/gtqmumcfzg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhengqikj.top/gtqcbvjhmj.html

[R25] 去后缀 / 去前缀
来源：http://hz.aizwys.cn/gtnilkspoq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jlsjyb.cn/gtvcsegflc.html

[R26] 命令替换
来源：http://hz.nanxuanxn.top/gtmmzirlvq.html

now=$(date +%F); echo "$now"
来源：http://hz.sufxvd.cn/gtqsnspjda.html

[R27] 算术展开
来源：http://hz.shanyushiyangtech.top/gtaerexgor.html

echo $((1 + 2 * 3))
来源：http://hz.zhengqikj.top/gtcexuajur.html

[R28] 浮点运算
来源：http://hz.aizwys.cn/gtnfrzyogg.html

echo "scale=2; 10/3" | bc
来源：http://hz.tianlin.xyz/gtlroklxrx.html

[R29] 定义函数
来源：http://hz.cheryme.top/gtlnqnqeex.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cucudq.cn/gtymkxkgdj.html

[R30] 函数返回状态码
来源：http://hz.svipenyu.cn/gtoshdsgop.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.havefunace.top/gtpbuesmbx.html

[R31] 局部变量
来源：http://hz.nwbrower.top/gtzgppoajg.html

f() { local x=1; echo "$x"; }
来源：http://hz.shanyushiyangkeji.top/gtefgodtth.html

[R32] 参数个数校验
来源：http://hz.sysykeji.top/gtbgdtsrke.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.daria6918.cn/gtuqbbufhi.html

[R33] 捕获错误并提示行号
来源：http://hz.vqdsnc.cn/gtxqmfzlnx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhongyouzk.top/gtvhqtydtq.html

[R34] 退出时清理
来源：http://hz.ywan-chungtsiang.top/gtgmbowlvx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yvedp.cn/gtmfophitg.html

[R35] 后台执行并等待
来源：http://hz.zhaomingkeji.xyz/gtrzemaglw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xingfuxueyuan.xyz/gtnmzednsa.html

[R36] 并发执行多个任务
来源：http://hz.jinqigufen.top/gtelwdnnbb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sufxvd.cn/gtrlcndfie.html

[R37] 把输出赋给变量
来源：http://hz.gotoacloud.top/gtrpniizlg.html

files=$(ls -1)
来源：http://hz.jyoumei.cn/gtitytiqyg.html

[R38] 管道串联
来源：http://hz.jinyuanbaomall.cn/gtxlnbwagv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgfzy.top/gtyebhgplz.html

[R39] 重定向标准输出与错误
来源：http://hz.yanxiufei.cn/gtprcjsgmc.html

cmd > out.log 2>&1
来源：http://hz.zhengqikj.top/gtkewajihu.html

[R40] 追加写日志
来源：http://hz.zhoulong.xyz/gtropofllp.html

echo "log" >> out.log
来源：http://hz.hfpthk.cn/gteusmsmhe.html

[R41] 丢弃输出
来源：http://hz.hysaishi.cn/gtaijuaygr.html

cmd >/dev/null 2>&1
来源：http://hz.kuanghao11.cn/gtwprfvflt.html

[R42] 输入重定向
来源：http://hz.haohaochexian.top/gtqezzhnvc.html

wc -l < a.txt
来源：http://hz.daxiang520.top/gtbamvmjya.html

[R43] 按名字查找文件
来源：http://hz.zhixingplan.top/gtqjduoexk.html

find . -name "*.log" -type f
来源：http://hz.yj202588.top/gtrimgxdak.html

[R44] 按修改时间查找
来源：http://hz.tanke756.top/gtesplzzbp.html

find . -mtime -7 -type f
来源：http://hz.jqgfzy.top/gtbomtfavt.html

[R45] 批量删除
来源：http://hz.dianchejie.cn/gtvovovhxd.html

find . -name "*.tmp" -delete
来源：http://hz.dianchejie.cn/gthbmskhuf.html

[R46] 递归替换文件内容
来源：http://hz.ppjwa.cn/gtjcjodedy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhongyouzk.top/gthjuqgzxx.html

[R47] sed 单行替换
来源：http://hz.jinghuilouyu.cn/gtlpfaxpwa.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.bjfxy.top/gtkmpouelc.html

[R48] awk 取指定列
来源：http://hz.0kj1m.cn/gtyulzjpsg.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhongyouzk.top/gtoeitarea.html

[R49] awk 带条件
来源：http://hz.vqdsnc.cn/gtkgjskouz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.smart0.xyz/gtozjvghht.html

[R50] awk 求和
来源：http://hz.c1oappe.top/gtsdxyeuta.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gotoacloud.top/gtkvztopdh.html

[R51] 排序去重取前几
来源：http://hz.sxryk.cn/gtzqbkhxqx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xziqi.cn/gthnrmccyc.html

[R52] 统计行数
来源：http://hz.chenjidiqi.icu/gtovuxrcms.html

wc -l a.txt
来源：http://hz.hongshengwenyu.top/gtxnpsjdzb.html

[R53] 查看文件头与实时尾
来源：http://hz.jinqigufen.top/gtwypfbzxl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhengqikj.top/gtovqnvxrz.html

[R54] 比较两个文件
来源：http://hz.pengpengdd.cyou/gtkpxyncib.html

diff a.txt b.txt
来源：http://hz.haohaochexian.top/gtoqxgliqm.html

[R55] 压缩与解压
来源：http://hz.zhengqikj.top/gtrhffgqxl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ybcxt.top/gttgabxjbp.html

[R56] 远程拷贝
来源：http://hz.andypj.xyz/gtasgpydrg.html

scp file user@host:/path/
来源：http://hz.smart0.xyz/gtgaktpihk.html

[R57] 远程执行命令
来源：http://hz.0kj1m.cn/gtwywkfapj.html

ssh user@host 'uptime'
来源：http://hz.zhoulong.xyz/gtoimfnkrb.html

[R58] 下载文件
来源：http://hz.xuanzx.com/gtebbwxjoq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jqgufenzy.top/gtnskvdanr.html

[R59] 发 POST JSON
来源：http://hz.xylfe.cn/gtplritylp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gaohongyu789.top/gtrbbnzrpo.html

[R60] 只看 HTTP 状态码
来源：http://hz.xinyue.icu/gtiovaawta.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tanke756.top/gtqhtmlock.html

[R61] 磁盘占用
来源：http://hz.ppjwa.cn/gtvtpoquqm.html

df -h;  du -sh *
来源：http://hz.dashuyun.cn/gtfkuzmxca.html

[R62] 找最占空间的文件
来源：http://hz.jqgfzy.top/gtcdfnvfpw.html

du -ah . | sort -rh | head -10
来源：http://hz.yangfankeji.com/gtvvnzldnm.html

[R63] 内存与进程
来源：http://hz.hfpthk.cn/gtjlnruzfh.html

free -h;  ps aux | grep nginx
来源：http://hz.yueranfly.top/gtrkvbkimv.html

[R64] 结束进程
来源：http://hz.ydzc1.top/gtzascysvy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.vqdsnc.cn/gtissdqyjk.html

[R65] 查看端口占用
来源：http://hz.hnqzz.top/gtavtarmho.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shzxlz.cn/gtpodqssiq.html

[R66] 定时任务
来源：http://hz.gogol.net.cn/gturrugyhq.html

crontab -e;  crontab -l
来源：http://hz.zhiwuduotai.top/gtxeysbjjn.html

[R67] 生成随机十六进制串
来源：http://hz.dashuyun.cn/gtnninpowf.html

openssl rand -hex 16
来源：http://hz.nanxuanxn.top/gtneapcllh.html

[R68] 计算文件校验值
来源：http://hz.hnqzz.top/gtheknhpkp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xuetiantiany.cn/gtcgjfkzih.html

[R69] 生成随机密码
来源：http://hz.yj20258888.top/gtxyklmxyv.html

head -c 16 /dev/urandom | base64
来源：http://hz.xylfe.cn/gtciumqbly.html

[R70] 时间戳与互转
来源：http://hz.guowangkeji.top/gtgpcprbbj.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258.top/gtobeuvdiu.html

[R71] 日期格式化
来源：http://hz.yonumen.top/gtsjzjahbq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sysykeji.top/gtxwcotwff.html

[R72] 等待端口就绪
来源：http://hz.pengpengdd.cyou/gttyjmudqb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ehwqpu.com/gtsujgptwz.html

[R73] 分割大日志
来源：http://hz.yonumen.top/gtzcmcconl.html

split -l 1000 big.log part_
来源：http://hz.bjfxy.top/gtwoobyfql.html

[R74] 批量重命名
来源：http://hz.pycfn.com/gtaldktkuf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sxryk.cn/gthjkoovdd.html

[R75] 导出环境变量
来源：http://hz.yj20258888.top/gthnifzsxk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yongpay.top/gtitkzmvfa.html

[R76] 使用临时文件
来源：http://hz.shangyingyoupin.top/gtwgfyqflf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhaomingkeji.xyz/gteqvaizgm.html

[R77] 读取用户输入
来源：http://hz.yangfankeji.com/gtzbpmbpsq.html

read -rp "请输入: " ans
来源：http://hz.jlsjyb.cn/gtrvzeygqz.html

[R78] 交互式菜单
来源：http://hz.dashuyun.cn/gtzqnzaxuw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hammf.cn/gtsgliuazj.html

[R79] 解析命令行选项
来源：http://hz.shzxlz.cn/gtrpnyqjah.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cqqwz.cn/gtsbxdwjhj.html

[R80] 查看脚本执行耗时
来源：http://hz.cdnleiting.top/gtkuywurrd.html

time ./run.sh
来源：http://hz.zhengqikj.top/gtygywhpzv.html

================================================================================
来源：http://hz.kuanghao11.cn/gtjwnpssga.html

S. C / C++ 专题
来源：http://hz.zhaomingkeji.xyz/gtduitzmpo.html

================================================================================
来源：http://hz.cdnleiting.top/gtgghgoopw.html

[S01] C：Hello World
来源：http://hz.tianlin.xyz/gttffpicrq.html

#include <stdio.h>
来源：http://hz.ywan-chungtsiang.top/gtxickiagd.html


<!-- 参考信息 -->