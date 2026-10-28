代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shzxlz.cn/gtxvoxiqpa.html

[Q26] 计数
来源：http://hz.guannengcc.top/gtbfvqopiy.html

SELECT COUNT(*) FROM users;
来源：http://hz.yuanzhike.top/gtrgfcjsvi.html

[Q27] 条件计数
来源：http://hz.svipenyu.cn/gtzlgasmvt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pengpengdd.cyou/gtzyccxjhd.html

[Q28] 求和与平均
来源：http://hz.fengsongda.top/gtdukmihdp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhengqikj.top/gtzpcnkwsa.html

[Q29] 最大最小值
来源：http://hz.jianghu66.top/gtisbyfrdz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.birdmap.top/gtjzdiclyy.html

[Q30] 分组统计
来源：http://hz.quarkkingdee.top/gtxesztelh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.dianchejie.cn/gtnrduitsp.html

[Q31] 分组后过滤
来源：http://hz.yanxiufei.cn/gtblwcpnhf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenjidiqi.icu/gtjkhwncgz.html

[Q32] 分组拼接字符串
来源：http://hz.hongshengwenyu.top/gtwalxozjz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jianghu66.top/gtweyrqzly.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.tanke756.top/gtbgnjkhmw.html

[Q33] 多列分组
来源：http://hz.shanyushiyangkeji.top/gtocrunpmh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.feifeiyinyue.top/gtmtdpecbl.html

[Q34] 每组取第一条
来源：http://hz.xuanzx.com/gtnyaniydp.html

SELECT * FROM (
来源：http://hz.yj202588.top/gtglmzockk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.52xcode.cn/gtmhusovhd.html

) t WHERE rn = 1;
来源：http://hz.zhixingplan.top/gtudfkhmtn.html

[Q35] 内连接
来源：http://hz.cashguo.top/gturqtsteg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnxiangtu.top/gtgaklsrtp.html

[Q36] 左连接
来源：http://hz.zycfv.cn/gtjfxvenrm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258888.top/gtxucnehxf.html

[Q37] 右连接
来源：http://hz.ydzc1.top/gtyrpispak.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.fzhhl.top/gtwqrgtfbd.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.52xcode.cn/gtlnxrqpgr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.wangdashe.top/gterlilfum.html

[Q39] 自连接（查上下级）
来源：http://hz.dashuyun.cn/gtjqdzrvta.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.snrcjt.cn/gtepphojnu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ppjwa.cn/gtinwvxpli.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cucudq.cn/gtlaienlgs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.316326.xyz/gtbuntldjd.html

[Q41] 多表连接
来源：http://hz.cashguo.top/gtowifsijp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cheryme.top/gtangaegsj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yueranfly.top/gteirghmxu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.daria6918.cn/gtidsheyrr.html

[Q42] 连接条件附加过滤
来源：http://hz.bjfxy.top/gttghenqdq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sxryk.cn/gtploemlrc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yj20258888.top/gtjhrwmozw.html

[Q43] 标量子查询
来源：http://hz.dashuyun.cn/gtkyckzydb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.kuanghao11.cn/gtuplsujvt.html

[Q44] IN 子查询
来源：http://hz.wangdashe.top/gtapzbokes.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhijiandao.cn/gtqkhzbxhn.html

[Q45] EXISTS 判断存在
来源：http://hz.dianchejie.cn/gtgsyougvi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xylfe.cn/gtatizjuia.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hongshengwenyu.top/gtlrxmcvaf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhaomingkeji.xyz/gtvvmpjyey.html

[Q47] 与平均值比较
来源：http://hz.gzhubu.top/gttxhypzlf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenzaomai.com/gtvtfmqxxl.html

[Q48] CTE 公用表表达式
来源：http://hz.fzhhl.top/gtfsyccyrf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.havefunace.top/gtmfjwselx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinqigfzy.top/gthomrlcsr.html

[Q49] 更新单行
来源：http://hz.chenjidiqi.icu/gtkwaygemh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhijiandao.cn/gtlusjbmra.html

[Q50] 批量更新
来源：http://hz.yj20258.top/gtftmobcpn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.smart0.xyz/gtxhgutkgf.html

[Q51] 用子查询更新
来源：http://hz.zhengqikj.top/gtghnznlhn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinqigfzy.top/gtveuhkril.html

[Q52] 删除指定行
来源：http://hz.yuxming.cn/gtctkefgii.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yangfankeji.com/gtcxnwggwr.html

[Q53] 按条件删除
来源：http://hz.dianchejie.cn/gtehxfbgrc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.bjfxy.top/gtkwofewpt.html

[Q54] 清空表
来源：http://hz.feifeiyinyue.top/gtohswlpoc.html

TRUNCATE TABLE logs;
来源：http://hz.xuanzx.com/gtcmsqdrvm.html

[Q55] 排名（并列占位）
来源：http://hz.zhongyouzk.top/gtweswslfh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zycfv.cn/gtmoaicsyb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hfpthk.cn/gticjzguui.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.snrcjt.cn/gtxyeydfkc.html

[Q57] 行号
来源：http://hz.cdnleiting.top/gtarqfvsgj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gzhubu.top/gtimntxdfy.html

[Q58] 累计求和
来源：http://hz.sysykeji.top/gtgizxbnpn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.pengpengdd.cyou/gtuzrdfxbb.html

[Q59] 分组内累计
来源：http://hz.jinghuilouyu.cn/gtizpywlxl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gogol.net.cn/gtrmlovjuo.html

[Q60] 取上一行 / 下一行
来源：http://hz.hnxiangtu.top/gtawbizgox.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jyoumei.cn/gtikdanqba.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yj202588.top/gtzwdkigjf.html

[Q61] 移动平均
来源：http://hz.xingfuxueyuan.xyz/gtkhlkidlf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.birdmap.top/gtantmkbma.html

[Q62] 分组占比
来源：http://hz.zhixingplan.top/gthyuzheul.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtolmvkrwd.html

[Q63] 开启事务
来源：http://hz.ywan-chungtsiang.top/gtptdsaszb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.daria6918.cn/gtruqvpwug.html

[Q64] 提交事务
来源：http://hz.yj20258.top/gttrtfxetd.html

COMMIT;
来源：http://hz.cashguo.top/gtotritowh.html

[Q65] 回滚事务
来源：http://hz.vqdsnc.cn/gtbbhabqby.html

ROLLBACK;
来源：http://hz.havefunace.top/gtrmkxjkzv.html

[Q66] 行锁查询
来源：http://hz.zhengqikj.top/gtdzdmxukm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sxryk.cn/gtntgcizom.html

[Q67] 设置隔离级别
来源：http://hz.hnqzz.top/gtiwijyhpb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.dashuyun.cn/gthnfnyivn.html

[Q68] 保存点
来源：http://hz.0kj1m.cn/gtoiwvbwss.html

SAVEPOINT sp1;
来源：http://hz.ehwqpu.com/gtncuxcbtp.html

ROLLBACK TO sp1;
来源：http://hz.kuanghao11.cn/gtqjzrcflg.html

[Q69] 查看执行计划
来源：http://hz.zhaomingkeji.xyz/gttdupkpjb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.feifeiyinyue.top/gtknlvwhrp.html

[Q70] 更新统计信息
来源：http://hz.yonumen.top/gtlculojra.html

ANALYZE TABLE users;
来源：http://hz.jiagoushi.top/gtzfdgdzaz.html

[Q71] 查看建表语句
来源：http://hz.meibo888.top/gtrdobrtsf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xuanzx.com/gtlwsqkjbv.html

[Q72] 查看索引
来源：http://hz.bjfxy.top/gtmcgbvexo.html

SHOW INDEX FROM users;
来源：http://hz.snrcjt.cn/gttabjjmth.html

[Q73] 查看表状态
来源：http://hz.cashguo.top/gtiriuyeck.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xuanzx.com/gthjlznvqc.html

[Q74] 强制使用索引
来源：http://hz.feifeiyinyue.top/gtewvvbemq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cheryme.top/gtvmvzszpi.html

[Q75] 日期格式化
来源：http://hz.nanxuanxn.top/gtfcehgkff.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ehwqpu.com/gtwfqqrawe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yangfankeji.com/gtptcrygkj.html

[Q76] 按天统计
来源：http://hz.aizwys.cn/gtqshnmict.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yj202588.top/gtppptfaaw.html

[Q77] 时间加减
来源：http://hz.jqgfzy.top/gtydxmrnmj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jqgfzy.top/gtqfnetevr.html

[Q78] 当前时间
来源：http://hz.birdmap.top/gtvjyuthkz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.fzhhl.top/gtprofzqad.html

[Q79] 字符串拼接
来源：http://hz.sysykeji.top/gtpiurjubi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hywenlv.cn/gtjsudcdij.html

[Q80] 字符串截取
来源：http://hz.shanyushiyangkeji.top/gtuytmxxuq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.316326.xyz/gtohbfhnjh.html

[Q81] 字符串替换
来源：http://hz.shanyushiyangkeji.top/gtbnxeolbh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.fengsongda.top/gtdtayliqm.html

[Q82] 字符长度与字节长度
来源：http://hz.zhengqikj.top/gtapggnynb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sweek.top/gtgchtynvb.html

[Q83] 大小写转换
来源：http://hz.zhongyouzk.top/gtevzjoxol.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.chenzaomai.com/gtvgmbtcyt.html

[Q84] 去除首尾空格
来源：http://hz.jiagoushi.top/gtfznisnam.html

SELECT TRIM(name) FROM users;
来源：http://hz.hywenlv.cn/gtikdpuebm.html

[Q85] 数值取整
来源：http://hz.hnxiangtu.top/gtpgmhkaia.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.aizwys.cn/gtlzzksmxt.html

[Q86] 读取 JSON 字段
来源：http://hz.hysaishi.cn/gtzkcyzril.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.daria6918.cn/gtgrqixydp.html

[Q87] JSON 字段做条件
来源：http://hz.tian-w.cn/gtsjfsixrz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.andypj.xyz/gtgsaqeeuu.html

[Q88] 行转列（条件聚合）
来源：http://hz.ivvv.top/gtnlwofocb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.havefunace.top/gtxmvhzhyk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ivvv.top/gttpfphhko.html

[Q89] 判断表是否存在
来源：http://hz.wangshuangyany.cn/gtlzyvicfl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinqigufen.top/gtlijxjmhm.html

[Q90] 生成序号列
来源：http://hz.cqqwz.cn/gtfslevsmi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.9152youxi.cn/gttmbxcled.html

================================================================================
来源：http://hz.ehwqpu.com/gtrluoyurv.html

R. Bash 专题
来源：http://hz.sufxvd.cn/gtgjlcqyzg.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtpqhxqlvt.html

[R01] shebang 与严格模式
来源：http://hz.52xcode.cn/gtzzxvtitu.html

#!/usr/bin/env bash
来源：http://hz.dashuyun.cn/gtkcqwtkyd.html

set -euo pipefail
来源：http://hz.yanxiufei.cn/gtpvpvibss.html

[R02] 变量赋值与使用
来源：http://hz.zycfv.cn/gtfgunbxvw.html

name="Tom"; echo "$name"
来源：http://hz.pycfn.com/gtbiklhpax.html

[R03] 只读变量
来源：http://hz.xingfuxueyuan.xyz/gtorjjezcb.html

readonly PI=3.14
来源：http://hz.daria6918.cn/gtrhfoyofz.html

[R04] 位置参数
来源：http://hz.tian-w.cn/gtzcdawrei.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yonumen.top/gttfpihlcj.html

[R05] 参数默认值
来源：http://hz.yuxming.cn/gtgcghcajt.html

name="${1:-default}"
来源：http://hz.xinyue.icu/gtsyrfcigt.html

[R06] 判断命令是否存在
来源：http://hz.gogol.net.cn/gtlmjlffop.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zdqjudy.top/gtvjthamcw.html

[R07] if 判断文件
来源：http://hz.shanyushiyangtech.top/gtnljudrjm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xinyue.icu/gtjnfyhyya.html

[R08] 数值比较
来源：http://hz.havefunace.top/gtumjgyauc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yvedp.cn/gtqndcktpt.html

[R09] 字符串比较
来源：http://hz.zhiwuduotai.top/gttxdguxjo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinqigufen.top/gtihcenbrk.html

[R10] 正则匹配
来源：http://hz.zhixingplan.top/gtehlykafr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ehwqpu.com/gtllhpoxtg.html

[R11] case 多分支
来源：http://hz.yonumen.top/gtbbkypgra.html

case "$1" in
来源：http://hz.tanke756.top/gtupdzurqb.html

start) echo "启动" ;;
来源：http://hz.xuanzx.com/gtrmszroei.html

stop)  echo "停止" ;;
来源：http://hz.jinqigufen.top/gtututxvjc.html

*)     echo "未知命令" ;;
来源：http://hz.dashuyun.cn/gtkmfujhoz.html

esac
来源：http://hz.sysykeji.top/gttneqisxb.html

[R12] for 遍历文件
来源：http://hz.birdmap.top/gtsviaeanq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.fzhhl.top/gtberxabyp.html

[R13] for 计数循环
来源：http://hz.shzxlz.cn/gtjvpmajii.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.birdmap.top/gtkopvxkag.html

[R14] C 风格 for
来源：http://hz.shuidangran.top/gtvitewsjv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.kuanghao11.cn/gttflyrfxs.html

[R15] while 逐行读文件
来源：http://hz.fengsongda.top/gtlguuovdn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hnxiangtu.top/gtbwmwctfc.html

[R16] until 等待条件
来源：http://hz.hongshengwenyu.top/gtbdyqlwfj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.9152youxi.cn/gtgeoprgwk.html

[R17] 数组定义与取值
来源：http://hz.fengsongda.top/gtrxphtxsc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hnxiangtu.top/gtfaccduuh.html

[R18] 遍历数组
来源：http://hz.ydjk.org.cn/gtfxxcfemk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinqigfzy.top/gtoqpkggru.html

[R19] 数组长度
来源：http://hz.zhiwuduotai.top/gtrdjsygsu.html

echo "${#arr[@]}"
来源：http://hz.chenzaomai.com/gtofshtrtr.html

[R20] 关联数组（字典）
来源：http://hz.ydzc1.top/gtqgebxkri.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hywenlv.cn/gtmbsdwrys.html

[R21] 字符串长度
来源：http://hz.tianlin.xyz/gtftmsqrvi.html

echo "${#s}"
来源：http://hz.guannengcc.top/gtdkclflbx.html

[R22] 截取子串
来源：http://hz.yvedp.cn/gtrrcewfwq.html

echo "${s:0:5}"
来源：http://hz.wangshuangyany.cn/gtdcvdkjzx.html

[R23] 字符串替换
来源：http://hz.snrcjt.cn/gtwkgrveay.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shuidangran.top/gtjerqtjir.html

[R24] 大小写转换
来源：http://hz.chenzaomai.com/gtrrgcgdui.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hnqzz.top/gtctamjwlf.html

[R25] 去后缀 / 去前缀
来源：http://hz.fzhhl.top/gtiexozqeg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.tanke756.top/gtvtltubda.html

[R26] 命令替换
来源：http://hz.feifeiyinyue.top/gtqjwzvkny.html

now=$(date +%F); echo "$now"
来源：http://hz.jianghu66.top/gtbifwcmws.html

[R27] 算术展开
来源：http://hz.zhaomingkeji.xyz/gtausdpbea.html

echo $((1 + 2 * 3))
来源：http://hz.andypj.xyz/gtynemnjfj.html

[R28] 浮点运算
来源：http://hz.xylfe.cn/gtnvzftrdr.html

echo "scale=2; 10/3" | bc
来源：http://hz.tianlin.xyz/gtckiqywmy.html

[R29] 定义函数
来源：http://hz.ehwqpu.com/gtsswbbtoc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.52xcode.cn/gtxljkyuqy.html

[R30] 函数返回状态码
来源：http://hz.shangyingyoupin.top/gtdiagkrgk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xuetiantiany.cn/gtklvaqvfc.html

[R31] 局部变量
来源：http://hz.wangshuangyany.cn/gtniognerh.html

f() { local x=1; echo "$x"; }
来源：http://hz.havefunace.top/gtidzsuuvr.html

[R32] 参数个数校验
来源：http://hz.gotoacloud.top/gtxhqcagjg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ydzc1.top/gtutmmmqtk.html

[R33] 捕获错误并提示行号
来源：http://hz.haohaochexian.top/gtbibbaimg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yvedp.cn/gttcburalz.html

[R34] 退出时清理
来源：http://hz.zdqjudy.top/gtoqnllgkf.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.svipenyu.cn/gtztjpfhpg.html

[R35] 后台执行并等待
来源：http://hz.guannengcc.top/gtvjkmryld.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhaomingkeji.xyz/gtvkrljkif.html

[R36] 并发执行多个任务
来源：http://hz.tianlin.xyz/gtoudpshhi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.nanxinkj.top/gtqmnobxhg.html

[R37] 把输出赋给变量
来源：http://hz.jinghuilouyu.cn/gtqntruilu.html

files=$(ls -1)
来源：http://hz.yj20258.top/gtwyalcsyd.html

[R38] 管道串联
来源：http://hz.ivvv.top/gthvbzwvji.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ywan-chungtsiang.top/gtohdjilwd.html

[R39] 重定向标准输出与错误
来源：http://hz.xziqi.cn/gtvzvjtbfq.html

cmd > out.log 2>&1
来源：http://hz.shanyushiyangtech.top/gtnmdflpex.html

[R40] 追加写日志
来源：http://hz.shangyingyoupin.top/gtcfxclckr.html

echo "log" >> out.log
来源：http://hz.hywenlv.cn/gtslzelbhu.html

[R41] 丢弃输出
来源：http://hz.shanyushiyangkeji.top/gtyfslnqmp.html

cmd >/dev/null 2>&1
来源：http://hz.hammf.cn/gtpnvzvuhu.html

[R42] 输入重定向
来源：http://hz.daria6918.cn/gtrsixwqvg.html

wc -l < a.txt
来源：http://hz.jiagoushi.top/gtvlodirbt.html

[R43] 按名字查找文件
来源：http://hz.shuidangran.top/gtkpvxwpwz.html

find . -name "*.log" -type f
来源：http://hz.zhoulong.xyz/gtcwovtmly.html

[R44] 按修改时间查找
来源：http://hz.feifeiyinyue.top/gtdspofukv.html

find . -mtime -7 -type f
来源：http://hz.cdnleiting.top/gtczhupljf.html

[R45] 批量删除
来源：http://hz.xziqi.cn/gtryikojzd.html

find . -name "*.tmp" -delete
来源：http://hz.hywenlv.cn/gtgzricjuz.html

[R46] 递归替换文件内容
来源：http://hz.0kj1m.cn/gtfztusykx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yangfankeji.com/gtaxweaqmg.html

[R47] sed 单行替换
来源：http://hz.sweek.top/gtvcsmcurc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.guowangkeji.top/gtbdmwwrwm.html

[R48] awk 取指定列
来源：http://hz.shanyushiyangkeji.top/gtcbpfhdkk.html

awk '{print $1, $3}' a.txt
来源：http://hz.aibaodan.cn/gtwbizuaca.html

[R49] awk 带条件
来源：http://hz.svipenyu.cn/gtoeqcsbpr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shanyushiyangkeji.top/gtvbzrxxcl.html

[R50] awk 求和
来源：http://hz.hammf.cn/gtpugeqvqp.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinqigufen.top/gtfpwkugnr.html

[R51] 排序去重取前几
来源：http://hz.hywenlv.cn/gtjujhrwvf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gogol.net.cn/gtfehgubla.html

[R52] 统计行数
来源：http://hz.kuanghao11.cn/gtdwevrvxe.html

wc -l a.txt
来源：http://hz.yuanzhike.top/gtfakrcjxl.html

[R53] 查看文件头与实时尾
来源：http://hz.svipenyu.cn/gtdbzwgjmk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenjidiqi.icu/gtnurnbadr.html

[R54] 比较两个文件
来源：http://hz.0kj1m.cn/gteqxucrgv.html

diff a.txt b.txt
来源：http://hz.ydjk.org.cn/gtqwhratva.html

[R55] 压缩与解压
来源：http://hz.chenjidiqi.icu/gtzqwbkuix.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hysaishi.cn/gtqtprvzub.html

[R56] 远程拷贝
来源：http://hz.guowangkeji.top/gthtyynklr.html

scp file user@host:/path/
来源：http://hz.hfpthk.cn/gtxramdlun.html

[R57] 远程执行命令
来源：http://hz.xuetiantiany.cn/gtgjsdtdpz.html

ssh user@host 'uptime'
来源：http://hz.yuanzhike.top/gtxxjlfvzo.html

[R58] 下载文件
来源：http://hz.feifeiyinyue.top/gtwimffirx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.kuanghao11.cn/gtdbpwxzvs.html

[R59] 发 POST JSON
来源：http://hz.sweek.top/gtdqkhcmgu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinghuilouyu.cn/gtzvttxjet.html

[R60] 只看 HTTP 状态码
来源：http://hz.yonumen.top/gtmjhybknr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.kuanghao11.cn/gtwjqvqbvu.html

[R61] 磁盘占用
来源：http://hz.hysaishi.cn/gtiuqfkhjo.html

df -h;  du -sh *
来源：http://hz.nanxuanxn.top/gtccteddrz.html

[R62] 找最占空间的文件
来源：http://hz.hysaishi.cn/gtherwuznk.html

du -ah . | sort -rh | head -10
来源：http://hz.shanyushiyangtech.top/gteopmbpve.html

[R63] 内存与进程
来源：http://hz.hfpthk.cn/gtcyyljtzj.html

free -h;  ps aux | grep nginx
来源：http://hz.fzhhl.top/gtendywjui.html

[R64] 结束进程
来源：http://hz.yuanzhike.top/gtlfklhbie.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenlongwang.top/gtgqcrglsj.html

[R65] 查看端口占用
来源：http://hz.yongpay.top/gtzfmxeptv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.pycfn.com/gtrtsmywyq.html

[R66] 定时任务
来源：http://hz.jinghuilouyu.cn/gtheszjrit.html

crontab -e;  crontab -l
来源：http://hz.cheryme.top/gtyffymyyi.html

[R67] 生成随机十六进制串
来源：http://hz.redwolf501.top/gtpeevmeit.html

openssl rand -hex 16
来源：http://hz.hnxiangtu.top/gtqigycvoj.html

[R68] 计算文件校验值
来源：http://hz.zycfv.cn/gtqsleafzr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gzhubu.top/gtyagzgycj.html

[R69] 生成随机密码
来源：http://hz.zhijiandao.cn/gtxqrarexk.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhaomingkeji.xyz/gtzdmpfsjy.html

[R70] 时间戳与互转
来源：http://hz.zhoulong.xyz/gtoxacgqyv.html

date +%s;  date -d @1700000000
来源：http://hz.shzxlz.cn/gtmnlkierz.html

[R71] 日期格式化
来源：http://hz.aibaodan.cn/gtkycyzdmy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.wangdashe.top/gtzmhonzqn.html

[R72] 等待端口就绪
来源：http://hz.jiagoushi.top/gtxzvqtvau.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydzc1.top/gtjkxeapnz.html

[R73] 分割大日志
来源：http://hz.snrcjt.cn/gtidedebvv.html

split -l 1000 big.log part_
来源：http://hz.ivvv.top/gtuavdmftj.html

[R74] 批量重命名
来源：http://hz.jqgufenzy.top/gtndblgdps.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.guannengcc.top/gtrorouujy.html

[R75] 导出环境变量
来源：http://hz.ydzc1.top/gtiukmcrki.html


<!-- 参考信息 -->