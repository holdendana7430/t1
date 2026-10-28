代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sweek.top/gtuuikclsb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhiwuduotai.top/gtvprbbfpm.html

[Q47] 与平均值比较
来源：http://hz.tanke756.top/gtbtbnooqe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yongpay.top/gtxulcodek.html

[Q48] CTE 公用表表达式
来源：http://hz.haohaochexian.top/gtpbawchwi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.fengsongda.top/gtrrpnmiih.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.feifeiyinyue.top/gtnhqlltxs.html

[Q49] 更新单行
来源：http://hz.c1oappe.top/gtohqrfgcc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.c1oappe.top/gtyunqfmas.html

[Q50] 批量更新
来源：http://hz.zhongyouzk.top/gtvbcdzkbk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jlsjyb.cn/gtmmkgnwyn.html

[Q51] 用子查询更新
来源：http://hz.hfpthk.cn/gtoyisiqic.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.guannengcc.top/gtvoxndlch.html

[Q52] 删除指定行
来源：http://hz.vqdsnc.cn/gtsghkxntx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zycfv.cn/gtsnaqdqbm.html

[Q53] 按条件删除
来源：http://hz.yueranfly.top/gtfsbqjcks.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhoulong.xyz/gtxhgxkojo.html

[Q54] 清空表
来源：http://hz.cucudq.cn/gtuftlhwuw.html

TRUNCATE TABLE logs;
来源：http://hz.sufxvd.cn/gtxruftgjk.html

[Q55] 排名（并列占位）
来源：http://hz.andypj.xyz/gtdobkbear.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.meibo888.top/gtfdjcjyim.html

[Q56] 密集排名（并列不占位）
来源：http://hz.wangshuangyany.cn/gtoiwyudgt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hammf.cn/gtyxunkmrt.html

[Q57] 行号
来源：http://hz.ywan-chungtsiang.top/gtkvklouag.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yonumen.top/gtqxemibgk.html

[Q58] 累计求和
来源：http://hz.yuanzhike.top/gtfpvuznju.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.meibo888.top/gtzalnzjcr.html

[Q59] 分组内累计
来源：http://hz.hammf.cn/gtxsyqosjy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.chenzaomai.com/gtxasmxyuk.html

[Q60] 取上一行 / 下一行
来源：http://hz.shanyushiyangkeji.top/gttqtdxzlx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangdashe.top/gtqakgtdta.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.mhx1999.top/gtknvtriat.html

[Q61] 移动平均
来源：http://hz.pycfn.com/gttwndactz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.haohaochexian.top/gtzkzdlauk.html

[Q62] 分组占比
来源：http://hz.meibo888.top/gtiapgxkrp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.smart0.xyz/gtagmsozhm.html

[Q63] 开启事务
来源：http://hz.shzxlz.cn/gtygydwraj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.fengsongda.top/gtjdsaksgo.html

[Q64] 提交事务
来源：http://hz.jinghuilouyu.cn/gtvriiboim.html

COMMIT;
来源：http://hz.52xcode.cn/gtyszhyjpz.html

[Q65] 回滚事务
来源：http://hz.jianghu66.top/gtqnbiauny.html

ROLLBACK;
来源：http://hz.jinqigufen.top/gtujxyjatr.html

[Q66] 行锁查询
来源：http://hz.zdqjudy.top/gttrjujhzx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.9152youxi.cn/gthqofnnav.html

[Q67] 设置隔离级别
来源：http://hz.yj20258888.top/gtezvcwhxn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.sysykeji.top/gtyxazimqy.html

[Q68] 保存点
来源：http://hz.xziqi.cn/gtczrnreyd.html

SAVEPOINT sp1;
来源：http://hz.jqgfzy.top/gtxxlvbhqb.html

ROLLBACK TO sp1;
来源：http://hz.guannengcc.top/gtsswctidu.html

[Q69] 查看执行计划
来源：http://hz.yvedp.cn/gtcxgcdihd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.aizwys.cn/gtycaunflp.html

[Q70] 更新统计信息
来源：http://hz.yvedp.cn/gtymdswywx.html

ANALYZE TABLE users;
来源：http://hz.dianchejie.cn/gtkkfunxga.html

[Q71] 查看建表语句
来源：http://hz.andypj.xyz/gtrdxuyaun.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ppjwa.cn/gtvrqltmeu.html

[Q72] 查看索引
来源：http://hz.aibaodan.cn/gtlusxvril.html

SHOW INDEX FROM users;
来源：http://hz.yuxming.cn/gtxpmuzdyf.html

[Q73] 查看表状态
来源：http://hz.xuetiantiany.cn/gtfxtisihl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jqgfzy.top/gtmlgarkko.html

[Q74] 强制使用索引
来源：http://hz.hfpthk.cn/gtonyiwifz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hnxiangtu.top/gtvmadbdxa.html

[Q75] 日期格式化
来源：http://hz.gogol.net.cn/gttdsthlzv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenzaomai.com/gtdaabchfe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.316326.xyz/gtwvtfcbtq.html

[Q76] 按天统计
来源：http://hz.yanxiufei.cn/gtaqoblpjz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.andypj.xyz/gtfwfwbauy.html

[Q77] 时间加减
来源：http://hz.jyoumei.cn/gtecgzbdvo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yj20258.top/gtjrbmizkl.html

[Q78] 当前时间
来源：http://hz.sxryk.cn/gtbdsnqdom.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.pycfn.com/gtuvkadyob.html

[Q79] 字符串拼接
来源：http://hz.havefunace.top/gttcnxvkio.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.0kj1m.cn/gtifbwbzyd.html

[Q80] 字符串截取
来源：http://hz.zhoulong.xyz/gtsmlhjghu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jqgufenzy.top/gtgvxqkrzz.html

[Q81] 字符串替换
来源：http://hz.gotoacloud.top/gtjjcbhsyw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.meibo888.top/gthvrjhogy.html

[Q82] 字符长度与字节长度
来源：http://hz.andypj.xyz/gtqapbqtzu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jqgfzy.top/gtvngrmpaw.html

[Q83] 大小写转换
来源：http://hz.fzhhl.top/gtnmzpbhzt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gogol.net.cn/gthewbpbqo.html

[Q84] 去除首尾空格
来源：http://hz.jinghuilouyu.cn/gtvoyzddnd.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtpuzxhioq.html

[Q85] 数值取整
来源：http://hz.0kj1m.cn/gtptgrdbmj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cqqwz.cn/gtcfevapom.html

[Q86] 读取 JSON 字段
来源：http://hz.tianlin.xyz/gtafotqing.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.haohaochexian.top/gtvpkzivxo.html

[Q87] JSON 字段做条件
来源：http://hz.tanke756.top/gtwvpsnuaw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.aibaodan.cn/gttkcgzded.html

[Q88] 行转列（条件聚合）
来源：http://hz.ppjwa.cn/gtzzwgcudj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yanxiufei.cn/gtfjardcfz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.9152youxi.cn/gtbpsffnmv.html

[Q89] 判断表是否存在
来源：http://hz.chenlongwang.top/gtqflxxjiw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.guowangkeji.top/gtrlzxrxgy.html

[Q90] 生成序号列
来源：http://hz.shanyushiyangkeji.top/gtxcunnmld.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.redwolf501.top/gtyukenwyf.html

================================================================================
来源：http://hz.wangdashe.top/gtbdmmkjiz.html

R. Bash 专题
来源：http://hz.snrcjt.cn/gtxjxapxjr.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtubexvzlk.html

[R01] shebang 与严格模式
来源：http://hz.cqqwz.cn/gttywhxict.html

#!/usr/bin/env bash
来源：http://hz.0kj1m.cn/gtkwxdelax.html

set -euo pipefail
来源：http://hz.nwbrower.top/gtsmpikwin.html

[R02] 变量赋值与使用
来源：http://hz.ybcxt.top/gtizewkczi.html

name="Tom"; echo "$name"
来源：http://hz.xziqi.cn/gtyvohdslj.html

[R03] 只读变量
来源：http://hz.pycfn.com/gtjneeqlph.html

readonly PI=3.14
来源：http://hz.xuanzx.com/gtknenbvfh.html

[R04] 位置参数
来源：http://hz.sysykeji.top/gtvujjlgzp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.meibo888.top/gtbkzprzvd.html

[R05] 参数默认值
来源：http://hz.hammf.cn/gtxbogpyep.html

name="${1:-default}"
来源：http://hz.vqdsnc.cn/gtxavflbfr.html

[R06] 判断命令是否存在
来源：http://hz.birdmap.top/gtcgfdtujp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gaohongyu789.top/gtkcpkxhey.html

[R07] if 判断文件
来源：http://hz.cucudq.cn/gtaszrdcvp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yanxiufei.cn/gtriirrzyh.html

[R08] 数值比较
来源：http://hz.wangshuangyany.cn/gtwmkivtyo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hfpthk.cn/gtiillnnft.html

[R09] 字符串比较
来源：http://hz.wangshuangyany.cn/gtpbiufvhy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sufxvd.cn/gtwjqbdtoe.html

[R10] 正则匹配
来源：http://hz.fzhhl.top/gtebeukvwm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj20258888.top/gtdypelyjv.html

[R11] case 多分支
来源：http://hz.hnxiangtu.top/gtxyagbpis.html

case "$1" in
来源：http://hz.yuanzhike.top/gtapinjuwi.html

start) echo "启动" ;;
来源：http://hz.cqqwz.cn/gtrqkyrokc.html

stop)  echo "停止" ;;
来源：http://hz.hywenlv.cn/gtlemocmqu.html

*)     echo "未知命令" ;;
来源：http://hz.yangfankeji.com/gtvhbzoihw.html

esac
来源：http://hz.chenzaomai.com/gtswodvwfn.html

[R12] for 遍历文件
来源：http://hz.chenjidiqi.icu/gtkmdggnnr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj20258888.top/gtdgzodlxf.html

[R13] for 计数循环
来源：http://hz.jinyuanbaomall.cn/gtoftnfoim.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.dianchejie.cn/gtgnbsyyhy.html

[R14] C 风格 for
来源：http://hz.wangdashe.top/gtzbcqidzd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.tian-w.cn/gtqzncrola.html

[R15] while 逐行读文件
来源：http://hz.52xcode.cn/gtjymwvsht.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hywenlv.cn/gtufemfcgo.html

[R16] until 等待条件
来源：http://hz.aizwys.cn/gtoyihjope.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.iojbl.cn/gtjerwvqvq.html

[R17] 数组定义与取值
来源：http://hz.jiagoushi.top/gtgklriksw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hnqzz.top/gtlwhbofrp.html

[R18] 遍历数组
来源：http://hz.hfpthk.cn/gtxxodgrzj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.tianlin.xyz/gtjrodfjae.html

[R19] 数组长度
来源：http://hz.hammf.cn/gtgmahxndp.html

echo "${#arr[@]}"
来源：http://hz.zhiwuduotai.top/gtlajqkzxe.html

[R20] 关联数组（字典）
来源：http://hz.jinghuilouyu.cn/gtfmdifsdh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shzxlz.cn/gtcjxkaglu.html

[R21] 字符串长度
来源：http://hz.jinqigufen.top/gtopnqeaob.html

echo "${#s}"
来源：http://hz.sweek.top/gtrzbjyset.html

[R22] 截取子串
来源：http://hz.daxiang520.top/gtmdelsluc.html

echo "${s:0:5}"
来源：http://hz.hnqzz.top/gtxxllvysm.html

[R23] 字符串替换
来源：http://hz.c1oappe.top/gtyrvapqvm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.nwbrower.top/gtyslybpkq.html

[R24] 大小写转换
来源：http://hz.xingfuxueyuan.xyz/gtyaqsdytd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jqgfzy.top/gtttoaaxev.html

[R25] 去后缀 / 去前缀
来源：http://hz.jianghu66.top/gtvuushjkl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shangyingyoupin.top/gtzrhqcxwk.html

[R26] 命令替换
来源：http://hz.yonumen.top/gtnmwqrpki.html

now=$(date +%F); echo "$now"
来源：http://hz.xuetiantiany.cn/gtucajmfkm.html

[R27] 算术展开
来源：http://hz.snrcjt.cn/gtyhxonlio.html

echo $((1 + 2 * 3))
来源：http://hz.yj20258888.top/gtsombwham.html

[R28] 浮点运算
来源：http://hz.andypj.xyz/gtrwcacwix.html

echo "scale=2; 10/3" | bc
来源：http://hz.jyoumei.cn/gtwcizfsmp.html

[R29] 定义函数
来源：http://hz.nanxuanxn.top/gtvqnffcgf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jyoumei.cn/gtosplompy.html

[R30] 函数返回状态码
来源：http://hz.redwolf501.top/gtugazggye.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ydzc1.top/gtzuxmfcxn.html

[R31] 局部变量
来源：http://hz.wangshuangyany.cn/gtjgvriuzt.html

f() { local x=1; echo "$x"; }
来源：http://hz.hongshengwenyu.top/gtvgrxadon.html

[R32] 参数个数校验
来源：http://hz.yj20258888.top/gthfuybtso.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sufxvd.cn/gtdzmfbxhl.html

[R33] 捕获错误并提示行号
来源：http://hz.52xcode.cn/gtuabegbsg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.52xcode.cn/gtozfxwopk.html

[R34] 退出时清理
来源：http://hz.sufxvd.cn/gtwzguncof.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinyuanbaomall.cn/gtnkdatiru.html

[R35] 后台执行并等待
来源：http://hz.ybcxt.top/gtecjcuozb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ybcxt.top/gtumyikwci.html

[R36] 并发执行多个任务
来源：http://hz.yj20258888.top/gtyfmpqfob.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xinyue.icu/gtnkeftqay.html

[R37] 把输出赋给变量
来源：http://hz.jyoumei.cn/gtibumhgxn.html

files=$(ls -1)
来源：http://hz.yonumen.top/gtgctwelbh.html

[R38] 管道串联
来源：http://hz.cqqwz.cn/gtzgjcclmr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jianghu66.top/gtcqvkhfgx.html

[R39] 重定向标准输出与错误
来源：http://hz.yj20258888.top/gtawkwztxe.html

cmd > out.log 2>&1
来源：http://hz.cucudq.cn/gtkqrxqbbb.html

[R40] 追加写日志
来源：http://hz.aibaodan.cn/gtbgzasrdu.html

echo "log" >> out.log
来源：http://hz.zhoulong.xyz/gteajavvcc.html

[R41] 丢弃输出
来源：http://hz.jinqigufen.top/gtghtiswjf.html

cmd >/dev/null 2>&1
来源：http://hz.ehwqpu.com/gttuvarijx.html

[R42] 输入重定向
来源：http://hz.shanyushiyangkeji.top/gtfusctedi.html

wc -l < a.txt
来源：http://hz.yj20258888.top/gtphncvvyf.html

[R43] 按名字查找文件
来源：http://hz.wangshuangyany.cn/gtjmgycmqf.html

find . -name "*.log" -type f
来源：http://hz.9152youxi.cn/gtmxcoowow.html

[R44] 按修改时间查找
来源：http://hz.pengpengdd.cyou/gtdayrbsop.html

find . -mtime -7 -type f
来源：http://hz.xuanzx.com/gtwmqcbvxa.html

[R45] 批量删除
来源：http://hz.snrcjt.cn/gtdiurpecl.html

find . -name "*.tmp" -delete
来源：http://hz.birdmap.top/gtlytqwgxo.html

[R46] 递归替换文件内容
来源：http://hz.0kj1m.cn/gtwsnieruf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.9152youxi.cn/gtxgeloltj.html

[R47] sed 单行替换
来源：http://hz.0kj1m.cn/gtrjljiefa.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yuxming.cn/gtwvaqrijb.html

[R48] awk 取指定列
来源：http://hz.pycfn.com/gtrwfmxhrd.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj20258.top/gtfqptkflr.html

[R49] awk 带条件
来源：http://hz.aizwys.cn/gtlcpejmqa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shanyushiyangtech.top/gtukfpzkiz.html

[R50] awk 求和
来源：http://hz.svipenyu.cn/gtrhrcindg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shanyushiyangtech.top/gtsuxowlzm.html

[R51] 排序去重取前几
来源：http://hz.nanxuanxn.top/gtepihrsvy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.wangdashe.top/gtdkjsstnl.html

[R52] 统计行数
来源：http://hz.yvedp.cn/gtrdapszcx.html

wc -l a.txt
来源：http://hz.yj20258.top/gtlssamudi.html

[R53] 查看文件头与实时尾
来源：http://hz.tianlin.xyz/gthshjrmxp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.52xcode.cn/gtmozxlpaw.html

[R54] 比较两个文件
来源：http://hz.jinghuilouyu.cn/gttymmkcfx.html

diff a.txt b.txt
来源：http://hz.ivvv.top/gtminueoem.html

[R55] 压缩与解压
来源：http://hz.yongpay.top/gtsigcrzfh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.52xcode.cn/gtseavdgai.html

[R56] 远程拷贝
来源：http://hz.c1oappe.top/gtghwtpcrt.html

scp file user@host:/path/
来源：http://hz.cheryme.top/gtcrbugyrq.html

[R57] 远程执行命令
来源：http://hz.ybcxt.top/gtzrstaykn.html

ssh user@host 'uptime'
来源：http://hz.hnxiangtu.top/gtdzoezdft.html

[R58] 下载文件
来源：http://hz.jlsjyb.cn/gtkbibvqaf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.wangdashe.top/gtyqxnbnuf.html

[R59] 发 POST JSON
来源：http://hz.ydjk.org.cn/gtdaripnft.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yongpay.top/gtfparmfew.html

[R60] 只看 HTTP 状态码
来源：http://hz.yongpay.top/gtxlnarpbn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.mhx1999.top/gtlsekphcx.html

[R61] 磁盘占用
来源：http://hz.feifeiyinyue.top/gtcahdrfjz.html

df -h;  du -sh *
来源：http://hz.jlsjyb.cn/gtnufyadfc.html

[R62] 找最占空间的文件
来源：http://hz.shanyushiyangtech.top/gtxniogujt.html

du -ah . | sort -rh | head -10
来源：http://hz.daxiang520.top/gtxurkfotb.html

[R63] 内存与进程
来源：http://hz.jiagoushi.top/gtqcozveoo.html

free -h;  ps aux | grep nginx
来源：http://hz.jlsjyb.cn/gttxyvfsyw.html

[R64] 结束进程
来源：http://hz.chenzaomai.com/gtzhesbqku.html

kill -9 $(pgrep -f app.py)
来源：http://hz.316326.xyz/gtobajtewx.html

[R65] 查看端口占用
来源：http://hz.hnqzz.top/gttodwzmmc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jqgfzy.top/gtgaizmkpt.html

[R66] 定时任务
来源：http://hz.birdmap.top/gtasjbdwur.html

crontab -e;  crontab -l
来源：http://hz.zdqjudy.top/gtikgbgfif.html

[R67] 生成随机十六进制串
来源：http://hz.havefunace.top/gtbqnzpton.html

openssl rand -hex 16
来源：http://hz.shanyushiyangkeji.top/gtxjfkzztd.html

[R68] 计算文件校验值
来源：http://hz.tanke756.top/gtdtmfevwj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.bjfxy.top/gtdnrtrwex.html

[R69] 生成随机密码
来源：http://hz.wangshuangyany.cn/gtpwxlaczl.html

head -c 16 /dev/urandom | base64
来源：http://hz.hnqzz.top/gtlflcwvth.html

[R70] 时间戳与互转
来源：http://hz.zhixingplan.top/gtfyonhbmq.html

date +%s;  date -d @1700000000
来源：http://hz.316326.xyz/gtcatvlhab.html

[R71] 日期格式化
来源：http://hz.xuetiantiany.cn/gtorpqgeck.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yj202588.top/gtotiydcvs.html

[R72] 等待端口就绪
来源：http://hz.andypj.xyz/gtmpsxfpqj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinqigufen.top/gtwcyulsdp.html

[R73] 分割大日志
来源：http://hz.yj20258.top/gtkazwvvlz.html

split -l 1000 big.log part_
来源：http://hz.9152youxi.cn/gtndcyvozy.html

[R74] 批量重命名
来源：http://hz.mhx1999.top/gtbpvdjwaq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zycfv.cn/gtzmxxyogx.html

[R75] 导出环境变量
来源：http://hz.guowangkeji.top/gtvsystzcq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ywan-chungtsiang.top/gtnsninxdq.html

[R76] 使用临时文件
来源：http://hz.wangshuangyany.cn/gtpryterfb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.birdmap.top/gtlnocepug.html

[R77] 读取用户输入
来源：http://hz.jianghu66.top/gtfrjuyavh.html

read -rp "请输入: " ans
来源：http://hz.tanke756.top/gtyifwgdoz.html

[R78] 交互式菜单
来源：http://hz.fzhhl.top/gtgcyyytdi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jiagoushi.top/gtrbuciswi.html

[R79] 解析命令行选项
来源：http://hz.pengpengdd.cyou/gtcllulzkc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shangyingyoupin.top/gtjbbclkdb.html

[R80] 查看脚本执行耗时
来源：http://hz.hfpthk.cn/gtrvhqqkwj.html

time ./run.sh
来源：http://hz.jinqigfzy.top/gtrjvdfawd.html

================================================================================
来源：http://hz.fengsongda.top/gtijeuvsmq.html

S. C / C++ 专题
来源：http://hz.haohaochexian.top/gtktxwkyom.html

================================================================================
来源：http://hz.ehwqpu.com/gtwgcjpzrx.html

[S01] C：Hello World
来源：http://hz.c1oappe.top/gtttqslowr.html

#include <stdio.h>
来源：http://hz.shanyushiyangkeji.top/gtfyofiehl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.bjfxy.top/gtmgeafzop.html

[S02] C：变量与格式化输出
来源：http://hz.xuanzx.com/gtdrmudwqm.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinqigfzy.top/gtlxyeapiu.html

[S03] C：读入整数
来源：http://hz.birdmap.top/gtxjgfrize.html

int x; scanf("%d", &x);
来源：http://hz.hysaishi.cn/gtjlmkqfur.html

[S04] C：字符串复制
来源：http://hz.shanyushiyangkeji.top/gtenzodlns.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nanxuanxn.top/gtxhxpmomm.html

[S05] C：字符串长度
来源：http://hz.jqgufenzy.top/gtbqpatbrx.html

strlen(s)
来源：http://hz.jinqigufen.top/gtnogusfpq.html

[S06] C：字符串比较
来源：http://hz.jinqigfzy.top/gtmvyykmuf.html

strcmp(a, b) == 0
来源：http://hz.daria6918.cn/gtnwiaonys.html

[S07] C：数组遍历求和
来源：http://hz.aibaodan.cn/gtmblajhtv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.kuanghao11.cn/gtevqgjzsw.html

[S08] C：动态内存分配与释放
来源：http://hz.shzxlz.cn/gtaoyblasl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.pengpengdd.cyou/gtypvuoxxh.html

[S09] C：结构体定义与初始化
来源：http://hz.tian-w.cn/gtuxtzlcul.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.kuanghao11.cn/gtovszwqxs.html

[S10] C：指针与解引用
来源：http://hz.gotoacloud.top/gtwxsmxtbh.html

int *p = &a;  *p = 5;
来源：http://hz.cqqwz.cn/gtgxqciijn.html

[S11] C：逐行读文件
来源：http://hz.tanke756.top/gtdgnpdzhp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.9152youxi.cn/gtawumswow.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sufxvd.cn/gtfuwawpok.html

fclose(f);
来源：http://hz.hnqzz.top/gtdjjxnrba.html

[S12] C：写文件
来源：http://hz.zhixingplan.top/gtmziqcurn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daxiang520.top/gteoftdoak.html

[S13] C：宏定义
来源：http://hz.shuidangran.top/gtkwldhlcb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nanxinkj.top/gtktpfgiii.html

[S14] C：枚举
来源：http://hz.cdnleiting.top/gtbdduwixg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhiwuduotai.top/gtffrjrdxj.html

[S15] C：类型转换
来源：http://hz.fengsongda.top/gtnuhtwdhm.html

(double) a / b
来源：http://hz.316326.xyz/gtuirtvpbr.html

[S16] C：位操作置位
来源：http://hz.jqgufenzy.top/gtexuqvcof.html


<!-- 参考信息 -->