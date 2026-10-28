代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.tian-w.cn/gtvaksxatx.html

) t WHERE rn = 1;
来源：http://hz.cashguo.top/gtpzucoedr.html

[Q35] 内连接
来源：http://hz.ydzc1.top/gtwtklfwhk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.quarkkingdee.top/gtyfvxkkoj.html

[Q36] 左连接
来源：http://hz.tanke756.top/gtrepuahpz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hfpthk.cn/gtnwvqgmke.html

[Q37] 右连接
来源：http://hz.feifeiyinyue.top/gteefnjgnr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.havefunace.top/gtbsxjsnmk.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shzxlz.cn/gtmubihuxn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hammf.cn/gtfgbmcuju.html

[Q39] 自连接（查上下级）
来源：http://hz.wangshuangyany.cn/gttrzrjefh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hnqzz.top/gtcukiezpk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.pycfn.com/gtqbadfifj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zycfv.cn/gtocwegdcu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shangyingyoupin.top/gtoyreitet.html

[Q41] 多表连接
来源：http://hz.gotoacloud.top/gtbiiaiiuu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhaomingkeji.xyz/gtdoaflgjl.html

JOIN users u ON u.id = o.user_id
来源：http://hz.bjfxy.top/gtjoepwgfl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.redwolf501.top/gtzgqdwwfy.html

[Q42] 连接条件附加过滤
来源：http://hz.jqgufenzy.top/gttyoiiemh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.vqdsnc.cn/gtabqjubyz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.vqdsnc.cn/gtwykbnqcg.html

[Q43] 标量子查询
来源：http://hz.9152youxi.cn/gtnzzdrncw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.9152youxi.cn/gttiejcote.html

[Q44] IN 子查询
来源：http://hz.pycfn.com/gtfjhbcuwh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yj202588.top/gtzfyednsp.html

[Q45] EXISTS 判断存在
来源：http://hz.gaohongyu789.top/gtinumclxq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jiagoushi.top/gtehyttour.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yonumen.top/gtoqhgdazm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhongyouzk.top/gtfjlesyey.html

[Q47] 与平均值比较
来源：http://hz.0kj1m.cn/gtsoxidyes.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hfpthk.cn/gtykrteege.html

[Q48] CTE 公用表表达式
来源：http://hz.yuanzhike.top/gtxfdvebwa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ybcxt.top/gtithzbqci.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinqigufen.top/gtmznyhsva.html

[Q49] 更新单行
来源：http://hz.jyoumei.cn/gtxaxhrfgq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.guannengcc.top/gtbfdnygxw.html

[Q50] 批量更新
来源：http://hz.zhixingplan.top/gtqhkcfujr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.aizwys.cn/gtihrzpvwj.html

[Q51] 用子查询更新
来源：http://hz.cashguo.top/gtbwkfzpdq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yuanzhike.top/gticsktgek.html

[Q52] 删除指定行
来源：http://hz.jlsjyb.cn/gtwxnjqbjj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yangfankeji.com/gtbzulevvc.html

[Q53] 按条件删除
来源：http://hz.c1oappe.top/gtpaspigng.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ivvv.top/gtgwqngmpo.html

[Q54] 清空表
来源：http://hz.xylfe.cn/gtetloayiv.html

TRUNCATE TABLE logs;
来源：http://hz.nanxinkj.top/gtxpsqadib.html

[Q55] 排名（并列占位）
来源：http://hz.cdnleiting.top/gtmmzecanb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ppjwa.cn/gtywsfiyog.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xuetiantiany.cn/gtlriqotvk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jiagoushi.top/gtsnkxpdar.html

[Q57] 行号
来源：http://hz.dianchejie.cn/gtiodntugc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.pycfn.com/gtpccecetn.html

[Q58] 累计求和
来源：http://hz.kuanghao11.cn/gtbcyuruks.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jyoumei.cn/gtinbxtpsy.html

[Q59] 分组内累计
来源：http://hz.yj20258888.top/gtfxkazjbd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cdnleiting.top/gtytgdanqb.html

[Q60] 取上一行 / 下一行
来源：http://hz.52xcode.cn/gtuuiifttv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.iojbl.cn/gtswrrxeqd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhixingplan.top/gtexpdbcxj.html

[Q61] 移动平均
来源：http://hz.zhoulong.xyz/gthgziwyec.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ppjwa.cn/gtfhvncrql.html

[Q62] 分组占比
来源：http://hz.snrcjt.cn/gtuukcuemh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtqfbsfbuf.html

[Q63] 开启事务
来源：http://hz.jinghuilouyu.cn/gtcnovfkgu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.quarkkingdee.top/gtrtegsrvd.html

[Q64] 提交事务
来源：http://hz.meibo888.top/gtwntjstso.html

COMMIT;
来源：http://hz.hnqzz.top/gtfpjaeono.html

[Q65] 回滚事务
来源：http://hz.vqdsnc.cn/gtfleohjjo.html

ROLLBACK;
来源：http://hz.fzhhl.top/gtboiydpvj.html

[Q66] 行锁查询
来源：http://hz.meibo888.top/gtgvmhprxb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.redwolf501.top/gtcoojuehy.html

[Q67] 设置隔离级别
来源：http://hz.gzhubu.top/gtiqmclayn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gotoacloud.top/gtuvpaghpq.html

[Q68] 保存点
来源：http://hz.aibaodan.cn/gtydtpwjwz.html

SAVEPOINT sp1;
来源：http://hz.hysaishi.cn/gtualpmxdp.html

ROLLBACK TO sp1;
来源：http://hz.guannengcc.top/gttnmkfnaa.html

[Q69] 查看执行计划
来源：http://hz.jinqigufen.top/gtlhuyjuju.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ivvv.top/gtcayzfzio.html

[Q70] 更新统计信息
来源：http://hz.vqdsnc.cn/gtagqwkbil.html

ANALYZE TABLE users;
来源：http://hz.ydzc1.top/gtjozgtyqc.html

[Q71] 查看建表语句
来源：http://hz.kuanghao11.cn/gtayzojnps.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cqqwz.cn/gtfaxofnxo.html

[Q72] 查看索引
来源：http://hz.yj20258888.top/gttgpmlxxv.html

SHOW INDEX FROM users;
来源：http://hz.cqqwz.cn/gtkxpbamuw.html

[Q73] 查看表状态
来源：http://hz.meibo888.top/gtxzxghubw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.haohaochexian.top/gtezfyfmmj.html

[Q74] 强制使用索引
来源：http://hz.cucudq.cn/gtdalntcqx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yongpay.top/gtkjbawfpa.html

[Q75] 日期格式化
来源：http://hz.cashguo.top/gtirsaubhr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ehwqpu.com/gtumizeigh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.havefunace.top/gtefupcfvu.html

[Q76] 按天统计
来源：http://hz.tianlin.xyz/gtnbzbnaqd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gogol.net.cn/gtbwxsipte.html

[Q77] 时间加减
来源：http://hz.zhiwuduotai.top/gtsjfiqqny.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenjidiqi.icu/gtsbtwrkap.html

[Q78] 当前时间
来源：http://hz.ehwqpu.com/gtxvpxidav.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.wangdashe.top/gtazydejny.html

[Q79] 字符串拼接
来源：http://hz.yangfankeji.com/gtdqiktphg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xylfe.cn/gtvkxpwlbi.html

[Q80] 字符串截取
来源：http://hz.sweek.top/gtgsbfmsie.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.aizwys.cn/gtkljmzhph.html

[Q81] 字符串替换
来源：http://hz.jinqigufen.top/gtcjospith.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydzc1.top/gtqrocrtit.html

[Q82] 字符长度与字节长度
来源：http://hz.tianlin.xyz/gtwfasmkdd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtaxzudyzp.html

[Q83] 大小写转换
来源：http://hz.hnxiangtu.top/gtdlyblbsg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yanxiufei.cn/gtulqbrdcj.html

[Q84] 去除首尾空格
来源：http://hz.52xcode.cn/gtrbmtvtwy.html

SELECT TRIM(name) FROM users;
来源：http://hz.andypj.xyz/gtsnvfpcko.html

[Q85] 数值取整
来源：http://hz.quarkkingdee.top/gtwywbgdiv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.dianchejie.cn/gtqsdfpwlf.html

[Q86] 读取 JSON 字段
来源：http://hz.ppjwa.cn/gtwajgfusj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ywan-chungtsiang.top/gtbpirwlso.html

[Q87] JSON 字段做条件
来源：http://hz.yj20258888.top/gtasqlotms.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj202588.top/gtzrkdoias.html

[Q88] 行转列（条件聚合）
来源：http://hz.hammf.cn/gtcqqjnnbz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.316326.xyz/gtzvyzvwjh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yuxming.cn/gthnikihjs.html

[Q89] 判断表是否存在
来源：http://hz.xinyue.icu/gtjqsmwdel.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jianghu66.top/gtdihjttut.html

[Q90] 生成序号列
来源：http://hz.havefunace.top/gtfigdysug.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yj202588.top/gtnevsjdjj.html

================================================================================
来源：http://hz.jianghu66.top/gtbauhvfcw.html

R. Bash 专题
来源：http://hz.52xcode.cn/gtsmejqcjv.html

================================================================================
来源：http://hz.gogol.net.cn/gtwpftqsvz.html

[R01] shebang 与严格模式
来源：http://hz.guannengcc.top/gtcdldaerj.html

#!/usr/bin/env bash
来源：http://hz.yueranfly.top/gtdpekaucd.html

set -euo pipefail
来源：http://hz.yvedp.cn/gtboipbrsc.html

[R02] 变量赋值与使用
来源：http://hz.jinghuilouyu.cn/gtipjxpjct.html

name="Tom"; echo "$name"
来源：http://hz.daxiang520.top/gtnqcumjyp.html

[R03] 只读变量
来源：http://hz.aizwys.cn/gtgrxtzscj.html

readonly PI=3.14
来源：http://hz.quarkkingdee.top/gtygppiewz.html

[R04] 位置参数
来源：http://hz.xylfe.cn/gttapfjqnl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.pycfn.com/gtgngimvfw.html

[R05] 参数默认值
来源：http://hz.yj202588.top/gtvbxlsock.html

name="${1:-default}"
来源：http://hz.redwolf501.top/gtsywtbppu.html

[R06] 判断命令是否存在
来源：http://hz.zhijiandao.cn/gtrixkmfpz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.wangshuangyany.cn/gtaofpmgdv.html

[R07] if 判断文件
来源：http://hz.tian-w.cn/gthdzlcgrk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gzhubu.top/gtpaxfxrxg.html

[R08] 数值比较
来源：http://hz.zhiwuduotai.top/gtvfloalxy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jiagoushi.top/gtyhxulzte.html

[R09] 字符串比较
来源：http://hz.hywenlv.cn/gtxabuvjyh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gaohongyu789.top/gtdpuzelgp.html

[R10] 正则匹配
来源：http://hz.hfpthk.cn/gtnuffnlkk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhengqikj.top/gtdxmqlqka.html

[R11] case 多分支
来源：http://hz.zhijiandao.cn/gtcmgxkuqm.html

case "$1" in
来源：http://hz.pycfn.com/gtohzllyuk.html

start) echo "启动" ;;
来源：http://hz.316326.xyz/gtcefmzlki.html

stop)  echo "停止" ;;
来源：http://hz.guowangkeji.top/gtfmoifjdj.html

*)     echo "未知命令" ;;
来源：http://hz.jyoumei.cn/gtvnduefat.html

esac
来源：http://hz.316326.xyz/gthkhvztod.html

[R12] for 遍历文件
来源：http://hz.cdnleiting.top/gtbweeadjr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj20258888.top/gtxkivuaor.html

[R13] for 计数循环
来源：http://hz.dianchejie.cn/gtupsemnvn.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.wangdashe.top/gthjqmjcfq.html

[R14] C 风格 for
来源：http://hz.yangfankeji.com/gtsyxghzpi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.mhx1999.top/gtvwivawqi.html

[R15] while 逐行读文件
来源：http://hz.zhongyouzk.top/gttalzexno.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.daxiang520.top/gttgmjcyrw.html

[R16] until 等待条件
来源：http://hz.quarkkingdee.top/gtftmpnswu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shangyingyoupin.top/gtsmmuxtue.html

[R17] 数组定义与取值
来源：http://hz.jiagoushi.top/gthsfvjpdw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.vqdsnc.cn/gtapadbgwf.html

[R18] 遍历数组
来源：http://hz.jqgufenzy.top/gtfllbapbx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.daria6918.cn/gtvhjeyeur.html

[R19] 数组长度
来源：http://hz.xziqi.cn/gtwlszxtpe.html

echo "${#arr[@]}"
来源：http://hz.nanxuanxn.top/gtkdxlluhu.html

[R20] 关联数组（字典）
来源：http://hz.yuxming.cn/gtpajwxykh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xuetiantiany.cn/gtovkkhyby.html

[R21] 字符串长度
来源：http://hz.gogol.net.cn/gtuwfhkevm.html

echo "${#s}"
来源：http://hz.yj20258888.top/gtmhfmfqjf.html

[R22] 截取子串
来源：http://hz.hammf.cn/gtygzuvubx.html

echo "${s:0:5}"
来源：http://hz.0kj1m.cn/gtqsoniqbd.html

[R23] 字符串替换
来源：http://hz.jinyuanbaomall.cn/gthcyvzwza.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.fengsongda.top/gtjvylipvo.html

[R24] 大小写转换
来源：http://hz.jqgfzy.top/gtxqdzcfcu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xylfe.cn/gtocaexkaq.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinqigfzy.top/gtwcvmmxgw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhoulong.xyz/gtzpmzsoti.html

[R26] 命令替换
来源：http://hz.hnqzz.top/gtgqlllpsr.html

now=$(date +%F); echo "$now"
来源：http://hz.redwolf501.top/gtnffhmmjv.html

[R27] 算术展开
来源：http://hz.0kj1m.cn/gtpeiqtomi.html

echo $((1 + 2 * 3))
来源：http://hz.xziqi.cn/gtaqxsukgi.html

[R28] 浮点运算
来源：http://hz.xingfuxueyuan.xyz/gtymzovtgo.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhiwuduotai.top/gtlpkmjkff.html

[R29] 定义函数
来源：http://hz.chenlongwang.top/gtihovrwyd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yanxiufei.cn/gtrjpcsoyt.html

[R30] 函数返回状态码
来源：http://hz.sufxvd.cn/gtgwkjtpec.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gotoacloud.top/gtpulhbfrg.html

[R31] 局部变量
来源：http://hz.yongpay.top/gtewodbcnh.html

f() { local x=1; echo "$x"; }
来源：http://hz.xingfuxueyuan.xyz/gtpllyanjs.html

[R32] 参数个数校验
来源：http://hz.ydzc1.top/gtvbuvfvyc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhoulong.xyz/gtkmeqxpku.html

[R33] 捕获错误并提示行号
来源：http://hz.mhx1999.top/gtfajqqetg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhiwuduotai.top/gtkdzunxws.html

[R34] 退出时清理
来源：http://hz.yanxiufei.cn/gtmldwpevi.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhaomingkeji.xyz/gtlzgufjub.html

[R35] 后台执行并等待
来源：http://hz.shangyingyoupin.top/gtfpcjiamn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.daria6918.cn/gtybgnamki.html

[R36] 并发执行多个任务
来源：http://hz.zycfv.cn/gtypzxpfnf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xuetiantiany.cn/gtqghlmuml.html

[R37] 把输出赋给变量
来源：http://hz.cdnleiting.top/gtxwxywsmp.html

files=$(ls -1)
来源：http://hz.yongpay.top/gtyymkrzar.html

[R38] 管道串联
来源：http://hz.dianchejie.cn/gtznegmufh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tian-w.cn/gtmpovjgka.html

[R39] 重定向标准输出与错误
来源：http://hz.yanxiufei.cn/gtbzvgqcka.html

cmd > out.log 2>&1
来源：http://hz.jyoumei.cn/gtuqzzksnl.html

[R40] 追加写日志
来源：http://hz.daxiang520.top/gtopejwori.html

echo "log" >> out.log
来源：http://hz.yj20258888.top/gtmsexkcjh.html

[R41] 丢弃输出
来源：http://hz.jinqigufen.top/gtfiifvusr.html

cmd >/dev/null 2>&1
来源：http://hz.xuetiantiany.cn/gtgmflvqgb.html

[R42] 输入重定向
来源：http://hz.cucudq.cn/gtnzyqetjx.html

wc -l < a.txt
来源：http://hz.xuetiantiany.cn/gtuerbxicf.html

[R43] 按名字查找文件
来源：http://hz.tianlin.xyz/gtijwyrepr.html

find . -name "*.log" -type f
来源：http://hz.quarkkingdee.top/gtelralvqq.html

[R44] 按修改时间查找
来源：http://hz.dashuyun.cn/gtndvumpcb.html

find . -mtime -7 -type f
来源：http://hz.tianlin.xyz/gtzrvtypjw.html

[R45] 批量删除
来源：http://hz.pycfn.com/gtmymfpwcv.html

find . -name "*.tmp" -delete
来源：http://hz.yanxiufei.cn/gtmewmngaw.html

[R46] 递归替换文件内容
来源：http://hz.zhoulong.xyz/gtqsufonzj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yvedp.cn/gtjszcoexr.html

[R47] sed 单行替换
来源：http://hz.yongpay.top/gtnhgxhdbj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jianghu66.top/gtiztntdtf.html

[R48] awk 取指定列
来源：http://hz.sweek.top/gtimzczyhd.html

awk '{print $1, $3}' a.txt
来源：http://hz.xuetiantiany.cn/gthlqbfnug.html

[R49] awk 带条件
来源：http://hz.feifeiyinyue.top/gtixdgimbx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.birdmap.top/gttnwosurw.html

[R50] awk 求和
来源：http://hz.jianghu66.top/gtdgwetdpw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.vqdsnc.cn/gtdsglsbwx.html

[R51] 排序去重取前几
来源：http://hz.pengpengdd.cyou/gtuwwfgemt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenjidiqi.icu/gtbhhsdhhj.html

[R52] 统计行数
来源：http://hz.zhixingplan.top/gtkpswlark.html

wc -l a.txt
来源：http://hz.chenlongwang.top/gtmpkzvgme.html

[R53] 查看文件头与实时尾
来源：http://hz.wangdashe.top/gtxxxkluba.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sxryk.cn/gtntbjdjcp.html

[R54] 比较两个文件
来源：http://hz.xuanzx.com/gtgletclgl.html

diff a.txt b.txt
来源：http://hz.sweek.top/gtjsrhstxz.html

[R55] 压缩与解压
来源：http://hz.yongpay.top/gtlyeerugn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sweek.top/gtimtsdmju.html

[R56] 远程拷贝
来源：http://hz.chenzaomai.com/gtuartnrtv.html

scp file user@host:/path/
来源：http://hz.nanxinkj.top/gtnggrdnfv.html

[R57] 远程执行命令
来源：http://hz.birdmap.top/gtfnrvwfxh.html

ssh user@host 'uptime'
来源：http://hz.dianchejie.cn/gtarwowfkv.html

[R58] 下载文件
来源：http://hz.gaohongyu789.top/gtvkfxivsk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xuanzx.com/gtxtxaxpkl.html

[R59] 发 POST JSON
来源：http://hz.zhijiandao.cn/gtifjgscdz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yvedp.cn/gtvhfdpvbh.html

[R60] 只看 HTTP 状态码
来源：http://hz.xingfuxueyuan.xyz/gtqhcqkvcs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hfpthk.cn/gtjamkfchi.html

[R61] 磁盘占用
来源：http://hz.tian-w.cn/gtcsgocpen.html

df -h;  du -sh *
来源：http://hz.aizwys.cn/gthtnbwhgb.html

[R62] 找最占空间的文件
来源：http://hz.fengsongda.top/gtmmcrghqj.html

du -ah . | sort -rh | head -10
来源：http://hz.jqgufenzy.top/gtuszforxt.html

[R63] 内存与进程
来源：http://hz.chenlongwang.top/gtlynzfden.html

free -h;  ps aux | grep nginx
来源：http://hz.meibo888.top/gtoeusohzv.html

[R64] 结束进程
来源：http://hz.shuidangran.top/gtrltzmxkd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj20258888.top/gtsqtfvqzd.html

[R65] 查看端口占用
来源：http://hz.hammf.cn/gthgzauwbo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinyuanbaomall.cn/gtamjpwkef.html

[R66] 定时任务
来源：http://hz.sufxvd.cn/gtpcqetmrg.html

crontab -e;  crontab -l
来源：http://hz.0kj1m.cn/gtuayanbod.html

[R67] 生成随机十六进制串
来源：http://hz.jyoumei.cn/gtmvohlxoj.html

openssl rand -hex 16
来源：http://hz.shangyingyoupin.top/gtbejpbwci.html

[R68] 计算文件校验值
来源：http://hz.0kj1m.cn/gtnzqsxxpp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenlongwang.top/gtquanxpzc.html

[R69] 生成随机密码
来源：http://hz.meibo888.top/gteesngqic.html

head -c 16 /dev/urandom | base64
来源：http://hz.yuanzhike.top/gtdyjatlof.html

[R70] 时间戳与互转
来源：http://hz.316326.xyz/gtxmlsvnyv.html

date +%s;  date -d @1700000000
来源：http://hz.hysaishi.cn/gthrhmogrt.html

[R71] 日期格式化
来源：http://hz.tanke756.top/gtjnlclmhg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.dianchejie.cn/gtdpnhqghf.html

[R72] 等待端口就绪
来源：http://hz.c1oappe.top/gtavhitlap.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xylfe.cn/gtbqshheml.html

[R73] 分割大日志
来源：http://hz.hongshengwenyu.top/gthirdascp.html

split -l 1000 big.log part_
来源：http://hz.iojbl.cn/gtbcfiifol.html

[R74] 批量重命名
来源：http://hz.gotoacloud.top/gtjzhaxaht.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xziqi.cn/gtoldborkq.html

[R75] 导出环境变量
来源：http://hz.daxiang520.top/gtijlsabcp.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xinyue.icu/gtezwsuyyh.html

[R76] 使用临时文件
来源：http://hz.fzhhl.top/gtanxjikps.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.0kj1m.cn/gtdjlgzyyd.html

[R77] 读取用户输入
来源：http://hz.smart0.xyz/gtbhsspiii.html

read -rp "请输入: " ans
来源：http://hz.cqqwz.cn/gttwaswqbx.html

[R78] 交互式菜单
来源：http://hz.c1oappe.top/gtgiymgzla.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xziqi.cn/gtjjeltwgt.html

[R79] 解析命令行选项
来源：http://hz.zhijiandao.cn/gtdfhvulep.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sysykeji.top/gtggyyyqss.html

[R80] 查看脚本执行耗时
来源：http://hz.aizwys.cn/gtuzqralxo.html

time ./run.sh
来源：http://hz.ywan-chungtsiang.top/gtgsuguhwx.html

================================================================================
来源：http://hz.52xcode.cn/gtjjhrnrsg.html

S. C / C++ 专题
来源：http://hz.yj20258.top/gtdmenglng.html

================================================================================
来源：http://hz.yj20258888.top/gtvoftpagb.html

[S01] C：Hello World
来源：http://hz.zhiwuduotai.top/gtafgqfzsx.html

#include <stdio.h>
来源：http://hz.yongpay.top/gtjsopgusq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.smart0.xyz/gtadqgnwfb.html

[S02] C：变量与格式化输出
来源：http://hz.yonumen.top/gtjivezcfg.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhoulong.xyz/gtswrgaiup.html

[S03] C：读入整数
来源：http://hz.sweek.top/gtevlrtsem.html


<!-- 参考信息 -->