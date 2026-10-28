代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.52xcode.cn/gtttkefwhy.html

[Q22] 排序
来源：http://hz.yj20258.top/gtsroeibzj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.guannengcc.top/gtqktmqxog.html

[Q23] 分页
来源：http://hz.aizwys.cn/gtvhjuiptq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhixingplan.top/gtayjglfxz.html

[Q24] 去重
来源：http://hz.hnqzz.top/gtnvmfrzqr.html

SELECT DISTINCT city FROM users;
来源：http://hz.yuanzhike.top/gtsifhlttj.html

[Q25] 只取前 N 条
来源：http://hz.mhx1999.top/gtjyarzjsw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.feifeiyinyue.top/gtgxbyhyjf.html

[Q26] 计数
来源：http://hz.guowangkeji.top/gtpxbpzmzm.html

SELECT COUNT(*) FROM users;
来源：http://hz.jiagoushi.top/gtrthrjanz.html

[Q27] 条件计数
来源：http://hz.aibaodan.cn/gtcmnptrod.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhixingplan.top/gtqfannxtk.html

[Q28] 求和与平均
来源：http://hz.daxiang520.top/gtbkrctfbb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.chenzaomai.com/gtxhweelzh.html

[Q29] 最大最小值
来源：http://hz.xziqi.cn/gtsvxempto.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yueranfly.top/gtmrgthzec.html

[Q30] 分组统计
来源：http://hz.hnqzz.top/gtpztdwyrs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hnxiangtu.top/gthfkmhmke.html

[Q31] 分组后过滤
来源：http://hz.zdqjudy.top/gtpsjomnhw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xziqi.cn/gttujutiun.html

[Q32] 分组拼接字符串
来源：http://hz.daria6918.cn/gtjmjictqq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtkgiwregm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yangfankeji.com/gtqpheszhp.html

[Q33] 多列分组
来源：http://hz.daxiang520.top/gtulchggwl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.kuanghao11.cn/gtzpsvigtp.html

[Q34] 每组取第一条
来源：http://hz.shangyingyoupin.top/gtamfmycpr.html

SELECT * FROM (
来源：http://hz.hammf.cn/gtqttazjfs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gogol.net.cn/gtbxhdtkre.html

) t WHERE rn = 1;
来源：http://hz.redwolf501.top/gtrovoplro.html

[Q35] 内连接
来源：http://hz.nanxuanxn.top/gtkhamnrll.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ivvv.top/gtdagfalny.html

[Q36] 左连接
来源：http://hz.zhaomingkeji.xyz/gtsowhxyka.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.316326.xyz/gtpjfvgdrm.html

[Q37] 右连接
来源：http://hz.zhoulong.xyz/gtuzaidhrt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.meibo888.top/gtdprvsqto.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.snrcjt.cn/gthoueisab.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hongshengwenyu.top/gthanljgzi.html

[Q39] 自连接（查上下级）
来源：http://hz.guannengcc.top/gthkfbkbau.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhongyouzk.top/gtbkzcnxgq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xuanzx.com/gtyzmmwufi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jlsjyb.cn/gtzaqexvby.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.tian-w.cn/gthbhvvjtu.html

[Q41] 多表连接
来源：http://hz.kuanghao11.cn/gtjiekrjba.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sufxvd.cn/gtqjovhubo.html

JOIN users u ON u.id = o.user_id
来源：http://hz.redwolf501.top/gtyweywivh.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.guannengcc.top/gtzkxrfmul.html

[Q42] 连接条件附加过滤
来源：http://hz.kuanghao11.cn/gtxlvufyxk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cdnleiting.top/gtkwvlvrnp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.9152youxi.cn/gtjvugymdf.html

[Q43] 标量子查询
来源：http://hz.hysaishi.cn/gtliyxnxbb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.svipenyu.cn/gtarwrfoub.html

[Q44] IN 子查询
来源：http://hz.sysykeji.top/gtdwanazta.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shanyushiyangtech.top/gtrjqrjtrw.html

[Q45] EXISTS 判断存在
来源：http://hz.ivvv.top/gtnkczomgu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cheryme.top/gtwpqoxyts.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.redwolf501.top/gtwcwlqlgi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.haohaochexian.top/gtzwjbyadi.html

[Q47] 与平均值比较
来源：http://hz.xziqi.cn/gtzhhfacxo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yvedp.cn/gtmqdztjdb.html

[Q48] CTE 公用表表达式
来源：http://hz.zdqjudy.top/gtpvugatxk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ydjk.org.cn/gtpuoemryy.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hysaishi.cn/gtohyburdn.html

[Q49] 更新单行
来源：http://hz.zhengqikj.top/gtxybeincw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yueranfly.top/gtkeddfadu.html

[Q50] 批量更新
来源：http://hz.cdnleiting.top/gtppbaielz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.fzhhl.top/gtfphqewsb.html

[Q51] 用子查询更新
来源：http://hz.fzhhl.top/gtotxspbfn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yueranfly.top/gtbgjvqxjb.html

[Q52] 删除指定行
来源：http://hz.ydzc1.top/gtczkyrqvg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gogol.net.cn/gtflqllggd.html

[Q53] 按条件删除
来源：http://hz.nanxinkj.top/gtfbpouvzg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jqgfzy.top/gtxvidplah.html

[Q54] 清空表
来源：http://hz.hywenlv.cn/gtbtllhyuj.html

TRUNCATE TABLE logs;
来源：http://hz.iojbl.cn/gtfwoaytxo.html

[Q55] 排名（并列占位）
来源：http://hz.shangyingyoupin.top/gtyblwnotu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yangfankeji.com/gtwkdyvzez.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nwbrower.top/gtnxhefujk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.chenlongwang.top/gtttxwyjib.html

[Q57] 行号
来源：http://hz.ydzc1.top/gtmehqqfkg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jqgufenzy.top/gtuufnwqmr.html

[Q58] 累计求和
来源：http://hz.cdnleiting.top/gtcnfxqwvo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.wangdashe.top/gtxlxfkxfg.html

[Q59] 分组内累计
来源：http://hz.yuanzhike.top/gthbkjyrmc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhoulong.xyz/gtggyqqime.html

[Q60] 取上一行 / 下一行
来源：http://hz.chenjidiqi.icu/gteeduhzdc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xuanzx.com/gtymawxhzc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zycfv.cn/gtazcujzxy.html

[Q61] 移动平均
来源：http://hz.cheryme.top/gtkeegzknw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.feifeiyinyue.top/gtfehsncau.html

[Q62] 分组占比
来源：http://hz.nanxuanxn.top/gtnoofiihz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cqqwz.cn/gtxstwvgib.html

[Q63] 开启事务
来源：http://hz.ydjk.org.cn/gtxuiikzjq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.andypj.xyz/gtbbbuunxm.html

[Q64] 提交事务
来源：http://hz.hongshengwenyu.top/gttddsydsm.html

COMMIT;
来源：http://hz.52xcode.cn/gtkmscwayh.html

[Q65] 回滚事务
来源：http://hz.cqqwz.cn/gtwejqwxjr.html

ROLLBACK;
来源：http://hz.shanyushiyangtech.top/gtqfeowwsg.html

[Q66] 行锁查询
来源：http://hz.jyoumei.cn/gtrxgelnla.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shzxlz.cn/gtkvbqdoni.html

[Q67] 设置隔离级别
来源：http://hz.cqqwz.cn/gtpgmnicqv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.tian-w.cn/gtlqwohqnq.html

[Q68] 保存点
来源：http://hz.52xcode.cn/gtctektkub.html

SAVEPOINT sp1;
来源：http://hz.cashguo.top/gtiehejyfs.html

ROLLBACK TO sp1;
来源：http://hz.yangfankeji.com/gtkdgydjkx.html

[Q69] 查看执行计划
来源：http://hz.zhoulong.xyz/gtbbxpxepk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.smart0.xyz/gtibsgvawj.html

[Q70] 更新统计信息
来源：http://hz.hammf.cn/gtbasbcnda.html

ANALYZE TABLE users;
来源：http://hz.hnxiangtu.top/gtpkbobpnn.html

[Q71] 查看建表语句
来源：http://hz.wangshuangyany.cn/gtuhlslwob.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yvedp.cn/gthyxgbfuc.html

[Q72] 查看索引
来源：http://hz.jianghu66.top/gtzpplpznt.html

SHOW INDEX FROM users;
来源：http://hz.jqgufenzy.top/gthnraevbc.html

[Q73] 查看表状态
来源：http://hz.sysykeji.top/gtwhtsdfmf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.guannengcc.top/gtuzcdqwye.html

[Q74] 强制使用索引
来源：http://hz.quarkkingdee.top/gtauslpfep.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.pengpengdd.cyou/gtddememlv.html

[Q75] 日期格式化
来源：http://hz.hongshengwenyu.top/gtfickaxmu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenlongwang.top/gtbajvmeqy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yueranfly.top/gtpidtqwqq.html

[Q76] 按天统计
来源：http://hz.gaohongyu789.top/gtlwxczkoh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ybcxt.top/gtpiclnhwv.html

[Q77] 时间加减
来源：http://hz.zhoulong.xyz/gtlacsepzy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.svipenyu.cn/gthcvpvkue.html

[Q78] 当前时间
来源：http://hz.redwolf501.top/gtbdenbbcx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sxryk.cn/gtrcbaqwxl.html

[Q79] 字符串拼接
来源：http://hz.cqqwz.cn/gtbngogdgn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cqqwz.cn/gtsyuukjag.html

[Q80] 字符串截取
来源：http://hz.yongpay.top/gtbmokufaz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sufxvd.cn/gtwerfehus.html

[Q81] 字符串替换
来源：http://hz.xuetiantiany.cn/gtlvqtmmhd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.dianchejie.cn/gtswqxbejo.html

[Q82] 字符长度与字节长度
来源：http://hz.svipenyu.cn/gtysrufqbx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hfpthk.cn/gtbedezeya.html

[Q83] 大小写转换
来源：http://hz.hfpthk.cn/gtjzwdazcd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.c1oappe.top/gtxgfsianf.html

[Q84] 去除首尾空格
来源：http://hz.fzhhl.top/gtfddabmoa.html

SELECT TRIM(name) FROM users;
来源：http://hz.fzhhl.top/gtzdakottn.html

[Q85] 数值取整
来源：http://hz.jinyuanbaomall.cn/gtbschsbkf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinyuanbaomall.cn/gtwhbwzvmk.html

[Q86] 读取 JSON 字段
来源：http://hz.ybcxt.top/gtkuefjyze.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenjidiqi.icu/gtmdtazonx.html

[Q87] JSON 字段做条件
来源：http://hz.jyoumei.cn/gtuavsdaze.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.andypj.xyz/gthraekvwp.html

[Q88] 行转列（条件聚合）
来源：http://hz.jqgfzy.top/gtyxhjsxsr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yvedp.cn/gtlarwaetf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.pycfn.com/gtyqyolqfw.html

[Q89] 判断表是否存在
来源：http://hz.nwbrower.top/gtiycwmibn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yongpay.top/gtfvxedkqu.html

[Q90] 生成序号列
来源：http://hz.cqqwz.cn/gtecixlkib.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jianghu66.top/gtrgikevet.html

================================================================================
来源：http://hz.ehwqpu.com/gtiusiybmc.html

R. Bash 专题
来源：http://hz.yj20258888.top/gtetpzosfl.html

================================================================================
来源：http://hz.ydjk.org.cn/gtdfebapgx.html

[R01] shebang 与严格模式
来源：http://hz.hnqzz.top/gthgxdnxlo.html

#!/usr/bin/env bash
来源：http://hz.yj20258.top/gtfyksmthi.html

set -euo pipefail
来源：http://hz.gogol.net.cn/gtnozihegs.html

[R02] 变量赋值与使用
来源：http://hz.nwbrower.top/gtkwlxxxvw.html

name="Tom"; echo "$name"
来源：http://hz.tanke756.top/gtlryktxuo.html

[R03] 只读变量
来源：http://hz.daria6918.cn/gtqswfpiwy.html

readonly PI=3.14
来源：http://hz.tian-w.cn/gtoktiwsdg.html

[R04] 位置参数
来源：http://hz.guowangkeji.top/gtkxekovlc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.havefunace.top/gtvfppabfn.html

[R05] 参数默认值
来源：http://hz.zhijiandao.cn/gtsisxdmtd.html

name="${1:-default}"
来源：http://hz.jinyuanbaomall.cn/gtvekpiuqt.html

[R06] 判断命令是否存在
来源：http://hz.shangyingyoupin.top/gtlcszoltw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.smart0.xyz/gtechisofb.html

[R07] if 判断文件
来源：http://hz.sysykeji.top/gtqvgmcsme.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.wangshuangyany.cn/gttessyyki.html

[R08] 数值比较
来源：http://hz.yanxiufei.cn/gtduwejmkd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.daxiang520.top/gtfxhmpmfy.html

[R09] 字符串比较
来源：http://hz.dashuyun.cn/gtfvsahnsw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hongshengwenyu.top/gtpbkxbyqi.html

[R10] 正则匹配
来源：http://hz.zhaomingkeji.xyz/gtqvnmqbdk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.fengsongda.top/gtsezdiqds.html

[R11] case 多分支
来源：http://hz.svipenyu.cn/gtiwhwgvwi.html

case "$1" in
来源：http://hz.bjfxy.top/gtprxxzdsz.html

start) echo "启动" ;;
来源：http://hz.xinyue.icu/gtznubbaif.html

stop)  echo "停止" ;;
来源：http://hz.zdqjudy.top/gtfhhykhus.html

*)     echo "未知命令" ;;
来源：http://hz.52xcode.cn/gtgqprvxvf.html

esac
来源：http://hz.vqdsnc.cn/gtquunfahf.html

[R12] for 遍历文件
来源：http://hz.hywenlv.cn/gthooaisql.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jiagoushi.top/gtzgqabpzo.html

[R13] for 计数循环
来源：http://hz.nanxinkj.top/gtofkdickp.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.smart0.xyz/gtnajgzzmz.html

[R14] C 风格 for
来源：http://hz.xingfuxueyuan.xyz/gtpcwggbwq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.iojbl.cn/gtebjvdrge.html

[R15] while 逐行读文件
来源：http://hz.bjfxy.top/gtumxgkvno.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tanke756.top/gtvdbulogg.html

[R16] until 等待条件
来源：http://hz.nanxuanxn.top/gtlpopqrjq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.chenjidiqi.icu/gtgwdnbted.html

[R17] 数组定义与取值
来源：http://hz.ivvv.top/gtkxvgnmzo.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yuxming.cn/gtyznxevub.html

[R18] 遍历数组
来源：http://hz.yueranfly.top/gtjhglxeob.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cqqwz.cn/gtdldmjvhn.html

[R19] 数组长度
来源：http://hz.zhixingplan.top/gtsbhbnsws.html

echo "${#arr[@]}"
来源：http://hz.guowangkeji.top/gtffjsmzgv.html

[R20] 关联数组（字典）
来源：http://hz.aibaodan.cn/gtrwqxmrgo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yangfankeji.com/gtvfbvzfgq.html

[R21] 字符串长度
来源：http://hz.hammf.cn/gtvulkdiyy.html

echo "${#s}"
来源：http://hz.zhengqikj.top/gtaagqrsoi.html

[R22] 截取子串
来源：http://hz.cdnleiting.top/gtccocbbfw.html

echo "${s:0:5}"
来源：http://hz.tian-w.cn/gtpuwibmtv.html

[R23] 字符串替换
来源：http://hz.dianchejie.cn/gtecntibbe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.iojbl.cn/gtazcghjrv.html

[R24] 大小写转换
来源：http://hz.cqqwz.cn/gtelnixgru.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.quarkkingdee.top/gtveugntci.html

[R25] 去后缀 / 去前缀
来源：http://hz.vqdsnc.cn/gtwhxcaaxt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.0kj1m.cn/gtwrwxjpfj.html

[R26] 命令替换
来源：http://hz.tianlin.xyz/gtlftttfln.html

now=$(date +%F); echo "$now"
来源：http://hz.yj202588.top/gtssismrkj.html

[R27] 算术展开
来源：http://hz.zhiwuduotai.top/gtjvdknmtm.html

echo $((1 + 2 * 3))
来源：http://hz.redwolf501.top/gtsocbharz.html

[R28] 浮点运算
来源：http://hz.zhiwuduotai.top/gticjxbxhi.html

echo "scale=2; 10/3" | bc
来源：http://hz.birdmap.top/gtlkdjirjy.html

[R29] 定义函数
来源：http://hz.cdnleiting.top/gtbbmbyxem.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jyoumei.cn/gtznwzgjqx.html

[R30] 函数返回状态码
来源：http://hz.yanxiufei.cn/gtvzavevyk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pengpengdd.cyou/gtjismvarg.html

[R31] 局部变量
来源：http://hz.chenlongwang.top/gtvjwfggju.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinghuilouyu.cn/gtzdkirasp.html

[R32] 参数个数校验
来源：http://hz.chenlongwang.top/gtyhxxpjyi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhijiandao.cn/gtoyekjalh.html

[R33] 捕获错误并提示行号
来源：http://hz.yueranfly.top/gteewpkkdm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.snrcjt.cn/gtdvjuxesj.html

[R34] 退出时清理
来源：http://hz.shzxlz.cn/gtivmwpzaj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtgavvvgaz.html

[R35] 后台执行并等待
来源：http://hz.bjfxy.top/gtccgddmgb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tianlin.xyz/gtdyeyhnpj.html

[R36] 并发执行多个任务
来源：http://hz.dashuyun.cn/gtjstsnsvq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.feifeiyinyue.top/gtbxrlnjng.html

[R37] 把输出赋给变量
来源：http://hz.nanxinkj.top/gthjiuohbw.html

files=$(ls -1)
来源：http://hz.sysykeji.top/gtnqejpnog.html

[R38] 管道串联
来源：http://hz.meibo888.top/gtagvuogjj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yuxming.cn/gtwjcwkheo.html

[R39] 重定向标准输出与错误
来源：http://hz.dianchejie.cn/gtglljhwkw.html

cmd > out.log 2>&1
来源：http://hz.jianghu66.top/gtlxnbdwrj.html

[R40] 追加写日志
来源：http://hz.jlsjyb.cn/gttvlgyizw.html

echo "log" >> out.log
来源：http://hz.meibo888.top/gtzngdfulc.html

[R41] 丢弃输出
来源：http://hz.ivvv.top/gtbdyyjlxc.html

cmd >/dev/null 2>&1
来源：http://hz.cqqwz.cn/gtoppbfdzg.html

[R42] 输入重定向
来源：http://hz.nanxuanxn.top/gtyedfcaqo.html

wc -l < a.txt
来源：http://hz.jyoumei.cn/gteqorchlp.html

[R43] 按名字查找文件
来源：http://hz.birdmap.top/gtnyttflnl.html

find . -name "*.log" -type f
来源：http://hz.9152youxi.cn/gtnxoetnhi.html

[R44] 按修改时间查找
来源：http://hz.ydjk.org.cn/gtbrvbqofi.html

find . -mtime -7 -type f
来源：http://hz.xylfe.cn/gtkommdrff.html

[R45] 批量删除
来源：http://hz.zhengqikj.top/gtipubangw.html

find . -name "*.tmp" -delete
来源：http://hz.bjfxy.top/gthpsscjuq.html

[R46] 递归替换文件内容
来源：http://hz.kuanghao11.cn/gtjzklxunr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.316326.xyz/gtxlfpvscq.html

[R47] sed 单行替换
来源：http://hz.smart0.xyz/gtdjjatlco.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhaomingkeji.xyz/gtdpnnidzl.html

[R48] awk 取指定列
来源：http://hz.xziqi.cn/gtaisblikg.html

awk '{print $1, $3}' a.txt
来源：http://hz.jqgufenzy.top/gtqksztlee.html

[R49] awk 带条件
来源：http://hz.zhengqikj.top/gtpxtvotmb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.birdmap.top/gtfwlzcjlv.html

[R50] awk 求和
来源：http://hz.9152youxi.cn/gtctfugvbe.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.feifeiyinyue.top/gtwsethoxa.html

[R51] 排序去重取前几
来源：http://hz.guannengcc.top/gtwhhhwiyc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.52xcode.cn/gtbdtdcmov.html

[R52] 统计行数
来源：http://hz.bjfxy.top/gtkcdefrbi.html

wc -l a.txt
来源：http://hz.yvedp.cn/gtwwzankvl.html

[R53] 查看文件头与实时尾
来源：http://hz.svipenyu.cn/gtgrbxsnlg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.aizwys.cn/gtyimcuktc.html

[R54] 比较两个文件
来源：http://hz.gogol.net.cn/gthxpvaaxr.html

diff a.txt b.txt
来源：http://hz.zhongyouzk.top/gthalukgfm.html

[R55] 压缩与解压
来源：http://hz.jinyuanbaomall.cn/gtjaavshzj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.quarkkingdee.top/gtarnelbmi.html

[R56] 远程拷贝
来源：http://hz.hnxiangtu.top/gttmvapurf.html

scp file user@host:/path/
来源：http://hz.yj202588.top/gtnjgcvrhw.html

[R57] 远程执行命令
来源：http://hz.chenjidiqi.icu/gtrhbahvgo.html

ssh user@host 'uptime'
来源：http://hz.yj20258.top/gtdjxcjigy.html

[R58] 下载文件
来源：http://hz.daxiang520.top/gtrfsvvhkc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.wangdashe.top/gtgwgwaozq.html

[R59] 发 POST JSON
来源：http://hz.shuidangran.top/gtycbdgdtz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shuidangran.top/gtqeonyqcm.html

[R60] 只看 HTTP 状态码
来源：http://hz.ehwqpu.com/gtslysadbp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hysaishi.cn/gtldsihypt.html

[R61] 磁盘占用
来源：http://hz.xylfe.cn/gtadezcsfy.html

df -h;  du -sh *
来源：http://hz.ppjwa.cn/gtpfpcdftx.html

[R62] 找最占空间的文件
来源：http://hz.gaohongyu789.top/gtqabfihwa.html

du -ah . | sort -rh | head -10
来源：http://hz.xingfuxueyuan.xyz/gtiwstqdyr.html

[R63] 内存与进程
来源：http://hz.cheryme.top/gtlveepidi.html

free -h;  ps aux | grep nginx
来源：http://hz.gotoacloud.top/gtzifpciex.html

[R64] 结束进程
来源：http://hz.zhixingplan.top/gtwuzcneda.html

kill -9 $(pgrep -f app.py)
来源：http://hz.haohaochexian.top/gtgxgioczh.html

[R65] 查看端口占用
来源：http://hz.havefunace.top/gtmmpatpva.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sxryk.cn/gtplpujjeg.html

[R66] 定时任务
来源：http://hz.xinyue.icu/gtxffbfppd.html

crontab -e;  crontab -l
来源：http://hz.jqgufenzy.top/gtjxzorrje.html

[R67] 生成随机十六进制串
来源：http://hz.guowangkeji.top/gtirclpofu.html

openssl rand -hex 16
来源：http://hz.yvedp.cn/gtqjiwidpo.html

[R68] 计算文件校验值
来源：http://hz.pycfn.com/gtwiirvpfq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cheryme.top/gtiatalkyl.html

[R69] 生成随机密码
来源：http://hz.ppjwa.cn/gtowqzsjhc.html

head -c 16 /dev/urandom | base64
来源：http://hz.redwolf501.top/gtufgewvzv.html

[R70] 时间戳与互转
来源：http://hz.jyoumei.cn/gtgbefairu.html

date +%s;  date -d @1700000000
来源：http://hz.chenlongwang.top/gtlufzlehe.html

[R71] 日期格式化
来源：http://hz.shanyushiyangtech.top/gtsqmvxylo.html


<!-- 参考信息 -->