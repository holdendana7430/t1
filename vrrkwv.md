代发 wailian999

[Q48] CTE 公用表表达式
来源：http://hz.iojbl.cn/gthfodldgg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.sufxvd.cn/gtryjobgaj.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yvedp.cn/gtlbrqbpyu.html

[Q49] 更新单行
来源：http://hz.havefunace.top/gtasbmpfbl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinghuilouyu.cn/gtgwliffvk.html

[Q50] 批量更新
来源：http://hz.tianlin.xyz/gtcwjsokvz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gogol.net.cn/gtijpltfut.html

[Q51] 用子查询更新
来源：http://hz.guannengcc.top/gtjiynlyfm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ehwqpu.com/gtglhiahsr.html

[Q52] 删除指定行
来源：http://hz.fzhhl.top/gttklasknu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sufxvd.cn/gtntwboxap.html

[Q53] 按条件删除
来源：http://hz.yanxiufei.cn/gtzrpkbuvs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yuanzhike.top/gtgwevisxy.html

[Q54] 清空表
来源：http://hz.gogol.net.cn/gtgfbhpnkc.html

TRUNCATE TABLE logs;
来源：http://hz.sxryk.cn/gtrcipwklb.html

[Q55] 排名（并列占位）
来源：http://hz.gotoacloud.top/gtaeliejrf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.snrcjt.cn/gtvfkeaodw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.chenzaomai.com/gtwqkytmwx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhijiandao.cn/gtdusxetay.html

[Q57] 行号
来源：http://hz.tianlin.xyz/gtkvspqelz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.pengpengdd.cyou/gtqlfnqqnz.html

[Q58] 累计求和
来源：http://hz.tian-w.cn/gthvutrxmp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ydzc1.top/gtgcinoppx.html

[Q59] 分组内累计
来源：http://hz.iojbl.cn/gtnsnaealu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hammf.cn/gtoxbjnsep.html

[Q60] 取上一行 / 下一行
来源：http://hz.zdqjudy.top/gtaodumobn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tianlin.xyz/gtmxpikgtt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hnqzz.top/gttypcibsf.html

[Q61] 移动平均
来源：http://hz.xinyue.icu/gtxmvijcng.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.daxiang520.top/gtokzpnmrl.html

[Q62] 分组占比
来源：http://hz.daxiang520.top/gtauzybtsq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtmmkainen.html

[Q63] 开启事务
来源：http://hz.hongshengwenyu.top/gtpovgqvtu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xuanzx.com/gtlpzoktkr.html

[Q64] 提交事务
来源：http://hz.yj20258.top/gtbsbehzvj.html

COMMIT;
来源：http://hz.iojbl.cn/gtkwmvzrkc.html

[Q65] 回滚事务
来源：http://hz.zhengqikj.top/gtllbioxvg.html

ROLLBACK;
来源：http://hz.guowangkeji.top/gtrvvqqwpf.html

[Q66] 行锁查询
来源：http://hz.jyoumei.cn/gtfipraqvs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.aibaodan.cn/gtnbfgldsz.html

[Q67] 设置隔离级别
来源：http://hz.jinqigfzy.top/gtkvceemus.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinghuilouyu.cn/gtcmakucjt.html

[Q68] 保存点
来源：http://hz.ppjwa.cn/gtytdcnefr.html

SAVEPOINT sp1;
来源：http://hz.yangfankeji.com/gtlpznprjj.html

ROLLBACK TO sp1;
来源：http://hz.pycfn.com/gtphrxfkbq.html

[Q69] 查看执行计划
来源：http://hz.iojbl.cn/gteaztbosn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ybcxt.top/gtukztxpvu.html

[Q70] 更新统计信息
来源：http://hz.jinghuilouyu.cn/gtubrjsclr.html

ANALYZE TABLE users;
来源：http://hz.jinghuilouyu.cn/gtiocrhqxn.html

[Q71] 查看建表语句
来源：http://hz.quarkkingdee.top/gtbxqbixhk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sxryk.cn/gtwakvxamd.html

[Q72] 查看索引
来源：http://hz.chenzaomai.com/gtpdagltwh.html

SHOW INDEX FROM users;
来源：http://hz.sweek.top/gticdekxwo.html

[Q73] 查看表状态
来源：http://hz.zhaomingkeji.xyz/gtjuhkqlkw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hysaishi.cn/gtfibkybsh.html

[Q74] 强制使用索引
来源：http://hz.daxiang520.top/gtluahzhgt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yj20258.top/gtyaecwboe.html

[Q75] 日期格式化
来源：http://hz.hfpthk.cn/gtbwgozths.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtgqtbuqlk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinqigufen.top/gtudwixwmi.html

[Q76] 按天统计
来源：http://hz.redwolf501.top/gtesmddaxt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yj20258.top/gtziqymdib.html

[Q77] 时间加减
来源：http://hz.0kj1m.cn/gtdrptwwxh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jqgfzy.top/gtushbgqnq.html

[Q78] 当前时间
来源：http://hz.sweek.top/gttfztckje.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xinyue.icu/gtugddgfiz.html

[Q79] 字符串拼接
来源：http://hz.ywan-chungtsiang.top/gtxjohjnwv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.fzhhl.top/gtmlqbhlla.html

[Q80] 字符串截取
来源：http://hz.redwolf501.top/gtduzrnmce.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinghuilouyu.cn/gtgujnieyy.html

[Q81] 字符串替换
来源：http://hz.cheryme.top/gtanbyruvy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnxiangtu.top/gtwpnygnyx.html

[Q82] 字符长度与字节长度
来源：http://hz.haohaochexian.top/gtzoubetgi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zycfv.cn/gtcxvhqfmp.html

[Q83] 大小写转换
来源：http://hz.smart0.xyz/gtprqpivxm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.havefunace.top/gtvhrswxev.html

[Q84] 去除首尾空格
来源：http://hz.zhoulong.xyz/gtcioohlzb.html

SELECT TRIM(name) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtuembsyxd.html

[Q85] 数值取整
来源：http://hz.zhiwuduotai.top/gtsdcjnehr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.chenjidiqi.icu/gtwvdeasee.html

[Q86] 读取 JSON 字段
来源：http://hz.xylfe.cn/gtjpshioyy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yuanzhike.top/gtunkwmyut.html

[Q87] JSON 字段做条件
来源：http://hz.52xcode.cn/gtskpfckrt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sweek.top/gtbfxwasyg.html

[Q88] 行转列（条件聚合）
来源：http://hz.xinyue.icu/gtwpxmfkoz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.316326.xyz/gtsopbgwbh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zdqjudy.top/gtsxeniemf.html

[Q89] 判断表是否存在
来源：http://hz.hnqzz.top/gtpopbqfci.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhengqikj.top/gtlaricodu.html

[Q90] 生成序号列
来源：http://hz.hnxiangtu.top/gtfjqdulhy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhaomingkeji.xyz/gthfkegole.html

================================================================================
来源：http://hz.fzhhl.top/gtqsmvhelt.html

R. Bash 专题
来源：http://hz.iojbl.cn/gtywekijel.html

================================================================================
来源：http://hz.sxryk.cn/gtrpigsfjv.html

[R01] shebang 与严格模式
来源：http://hz.nanxinkj.top/gtsxxgzetd.html

#!/usr/bin/env bash
来源：http://hz.haohaochexian.top/gtcopgdlgl.html

set -euo pipefail
来源：http://hz.meibo888.top/gtafvzrtbt.html

[R02] 变量赋值与使用
来源：http://hz.jiagoushi.top/gtowfrpzxi.html

name="Tom"; echo "$name"
来源：http://hz.zycfv.cn/gtwvabzbnn.html

[R03] 只读变量
来源：http://hz.chenlongwang.top/gtcamketmg.html

readonly PI=3.14
来源：http://hz.shzxlz.cn/gtshzalpcp.html

[R04] 位置参数
来源：http://hz.gzhubu.top/gtxogotofl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinghuilouyu.cn/gtawqrcqbg.html

[R05] 参数默认值
来源：http://hz.gzhubu.top/gtrenobuen.html

name="${1:-default}"
来源：http://hz.yueranfly.top/gtlzhhiptm.html

[R06] 判断命令是否存在
来源：http://hz.hywenlv.cn/gtzdazmlde.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.guowangkeji.top/gtqaubavel.html

[R07] if 判断文件
来源：http://hz.sysykeji.top/gtmbtnaxey.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gogol.net.cn/gtrwmirqnk.html

[R08] 数值比较
来源：http://hz.redwolf501.top/gtqmflbdge.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jyoumei.cn/gtffwrytoh.html

[R09] 字符串比较
来源：http://hz.xziqi.cn/gtrfplnqap.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.andypj.xyz/gtdozddylo.html

[R10] 正则匹配
来源：http://hz.chenzaomai.com/gttmwjptmm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.fengsongda.top/gttgxlxhow.html

[R11] case 多分支
来源：http://hz.hnqzz.top/gtppeodndk.html

case "$1" in
来源：http://hz.yueranfly.top/gtpaqnvkpb.html

start) echo "启动" ;;
来源：http://hz.jiagoushi.top/gtjntqyewv.html

stop)  echo "停止" ;;
来源：http://hz.shanyushiyangkeji.top/gtojnhpcgz.html

*)     echo "未知命令" ;;
来源：http://hz.zycfv.cn/gtvxbqwalz.html

esac
来源：http://hz.nanxuanxn.top/gtdmrvmsyh.html

[R12] for 遍历文件
来源：http://hz.chenzaomai.com/gtycpdqnqo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hfpthk.cn/gtaeprzcat.html

[R13] for 计数循环
来源：http://hz.haohaochexian.top/gttmxgaskn.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xziqi.cn/gtriuwlzbi.html

[R14] C 风格 for
来源：http://hz.jqgfzy.top/gtrvmqydzb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinyuanbaomall.cn/gtpkbmzgmi.html

[R15] while 逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtrpdtofre.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj20258.top/gtgpevaxyt.html

[R16] until 等待条件
来源：http://hz.ywan-chungtsiang.top/gtfakspuuf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.iojbl.cn/gtfzbiompr.html

[R17] 数组定义与取值
来源：http://hz.fengsongda.top/gttktnpvwq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.havefunace.top/gtkeusfzan.html

[R18] 遍历数组
来源：http://hz.tanke756.top/gtrmbfuzue.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yonumen.top/gtxfcyxrjl.html

[R19] 数组长度
来源：http://hz.yuxming.cn/gtxsmqmpdn.html

echo "${#arr[@]}"
来源：http://hz.zhoulong.xyz/gtdzyzznpt.html

[R20] 关联数组（字典）
来源：http://hz.sweek.top/gtubrflcam.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.52xcode.cn/gtcayowbth.html

[R21] 字符串长度
来源：http://hz.xylfe.cn/gtlklolrum.html

echo "${#s}"
来源：http://hz.wangdashe.top/gtnrhiugrj.html

[R22] 截取子串
来源：http://hz.ivvv.top/gtwlljphbe.html

echo "${s:0:5}"
来源：http://hz.zhoulong.xyz/gtynmojeeu.html

[R23] 字符串替换
来源：http://hz.hfpthk.cn/gtyabyhuly.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cucudq.cn/gtqyeyreho.html

[R24] 大小写转换
来源：http://hz.zhiwuduotai.top/gtdejqvcws.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.aibaodan.cn/gtquiqhtng.html

[R25] 去后缀 / 去前缀
来源：http://hz.hfpthk.cn/gtxtbkcjqy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.pycfn.com/gtbzwfppze.html

[R26] 命令替换
来源：http://hz.jlsjyb.cn/gtjhfiankm.html

now=$(date +%F); echo "$now"
来源：http://hz.ppjwa.cn/gtgxhrnzpa.html

[R27] 算术展开
来源：http://hz.iojbl.cn/gtikvjykfp.html

echo $((1 + 2 * 3))
来源：http://hz.bjfxy.top/gtpqgrwbkt.html

[R28] 浮点运算
来源：http://hz.hfpthk.cn/gtusgfxbir.html

echo "scale=2; 10/3" | bc
来源：http://hz.feifeiyinyue.top/gtyqnbbyps.html

[R29] 定义函数
来源：http://hz.daria6918.cn/gtwskwnsuq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.aizwys.cn/gttpytmzva.html

[R30] 函数返回状态码
来源：http://hz.shzxlz.cn/gtrhvugcrq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.redwolf501.top/gtauqvqgkp.html

[R31] 局部变量
来源：http://hz.guannengcc.top/gtguukzijk.html

f() { local x=1; echo "$x"; }
来源：http://hz.cucudq.cn/gtxfiemwrd.html

[R32] 参数个数校验
来源：http://hz.jqgufenzy.top/gtzpxweyxb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xuanzx.com/gtufwbydlx.html

[R33] 捕获错误并提示行号
来源：http://hz.jinqigfzy.top/gtjxvanuwt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinghuilouyu.cn/gtoshdjmam.html

[R34] 退出时清理
来源：http://hz.wangdashe.top/gtukztkdga.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangdashe.top/gtrwbkfrgx.html

[R35] 后台执行并等待
来源：http://hz.tian-w.cn/gtjzfujqor.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sxryk.cn/gtegubswdg.html

[R36] 并发执行多个任务
来源：http://hz.jinghuilouyu.cn/gtsdigcrac.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cashguo.top/gtztrdafgq.html

[R37] 把输出赋给变量
来源：http://hz.zdqjudy.top/gtbuzhuzuv.html

files=$(ls -1)
来源：http://hz.birdmap.top/gtfehgbioj.html

[R38] 管道串联
来源：http://hz.dashuyun.cn/gtddcnvrnt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hnxiangtu.top/gtcijmqemc.html

[R39] 重定向标准输出与错误
来源：http://hz.sweek.top/gttrmymkou.html

cmd > out.log 2>&1
来源：http://hz.ydzc1.top/gtcfmrgspl.html

[R40] 追加写日志
来源：http://hz.mhx1999.top/gtyuihsufe.html

echo "log" >> out.log
来源：http://hz.kuanghao11.cn/gtlfnryahu.html

[R41] 丢弃输出
来源：http://hz.haohaochexian.top/gtagvaqnrj.html

cmd >/dev/null 2>&1
来源：http://hz.52xcode.cn/gtcngvfxzb.html

[R42] 输入重定向
来源：http://hz.smart0.xyz/gtuqszmytc.html

wc -l < a.txt
来源：http://hz.gaohongyu789.top/gtdaovrfsg.html

[R43] 按名字查找文件
来源：http://hz.zhengqikj.top/gtekyewlnh.html

find . -name "*.log" -type f
来源：http://hz.jlsjyb.cn/gtkkoswvse.html

[R44] 按修改时间查找
来源：http://hz.yvedp.cn/gtgemeslgv.html

find . -mtime -7 -type f
来源：http://hz.gzhubu.top/gtvbgmqrzu.html

[R45] 批量删除
来源：http://hz.yuxming.cn/gtcisiiyrb.html

find . -name "*.tmp" -delete
来源：http://hz.52xcode.cn/gtaclzsadf.html

[R46] 递归替换文件内容
来源：http://hz.gogol.net.cn/gtwdqvdtur.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xinyue.icu/gtsjqzijfj.html

[R47] sed 单行替换
来源：http://hz.shuidangran.top/gtlwdepvmx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.smart0.xyz/gtqnjyhfqi.html

[R48] awk 取指定列
来源：http://hz.kuanghao11.cn/gtshbmfomn.html

awk '{print $1, $3}' a.txt
来源：http://hz.vqdsnc.cn/gtunltkdvi.html

[R49] awk 带条件
来源：http://hz.chenzaomai.com/gtdscebcqx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nwbrower.top/gtybmzubmv.html

[R50] awk 求和
来源：http://hz.snrcjt.cn/gttjqxhqxd.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtqmbmhtrs.html

[R51] 排序去重取前几
来源：http://hz.sysykeji.top/gtjinzacro.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.vqdsnc.cn/gttdxitvym.html

[R52] 统计行数
来源：http://hz.wangdashe.top/gtzmhiebgy.html

wc -l a.txt
来源：http://hz.zhoulong.xyz/gtjghprmdx.html

[R53] 查看文件头与实时尾
来源：http://hz.yongpay.top/gtvcryepio.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.guowangkeji.top/gtvvetmpvg.html

[R54] 比较两个文件
来源：http://hz.xylfe.cn/gtchyzxbpd.html

diff a.txt b.txt
来源：http://hz.pengpengdd.cyou/gtamwjggur.html

[R55] 压缩与解压
来源：http://hz.yuxming.cn/gtgcsjtnkr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.chenjidiqi.icu/gtxqtqyoty.html

[R56] 远程拷贝
来源：http://hz.nanxuanxn.top/gtajbmiqga.html

scp file user@host:/path/
来源：http://hz.52xcode.cn/gtahfqzuui.html

[R57] 远程执行命令
来源：http://hz.yueranfly.top/gtgjvadzqc.html

ssh user@host 'uptime'
来源：http://hz.xingfuxueyuan.xyz/gtxvyiibtl.html

[R58] 下载文件
来源：http://hz.gotoacloud.top/gthjdalfsf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cucudq.cn/gtkstdkqsf.html

[R59] 发 POST JSON
来源：http://hz.kuanghao11.cn/gtloiafreg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.haohaochexian.top/gtotasziqp.html

[R60] 只看 HTTP 状态码
来源：http://hz.gotoacloud.top/gtypmqobyz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.9152youxi.cn/gtklrbaxpv.html

[R61] 磁盘占用
来源：http://hz.iojbl.cn/gtfiqvhsad.html

df -h;  du -sh *
来源：http://hz.havefunace.top/gttskzxbid.html

[R62] 找最占空间的文件
来源：http://hz.yuxming.cn/gtwxdudqdh.html

du -ah . | sort -rh | head -10
来源：http://hz.sweek.top/gtfkmuffkc.html

[R63] 内存与进程
来源：http://hz.shzxlz.cn/gtokiwybwh.html

free -h;  ps aux | grep nginx
来源：http://hz.jyoumei.cn/gtojbmkbtr.html

[R64] 结束进程
来源：http://hz.snrcjt.cn/gtxnqnfsex.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj202588.top/gtyskvuxye.html

[R65] 查看端口占用
来源：http://hz.redwolf501.top/gtmzkqjdds.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinghuilouyu.cn/gtjjmzywnz.html

[R66] 定时任务
来源：http://hz.ehwqpu.com/gtnaydsgjn.html

crontab -e;  crontab -l
来源：http://hz.yueranfly.top/gtzxiccdjt.html

[R67] 生成随机十六进制串
来源：http://hz.pycfn.com/gtqogmqsya.html

openssl rand -hex 16
来源：http://hz.quarkkingdee.top/gtrjnrfybk.html

[R68] 计算文件校验值
来源：http://hz.yvedp.cn/gtdzupvglp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.havefunace.top/gtewxslhwp.html

[R69] 生成随机密码
来源：http://hz.guannengcc.top/gtbubiwusd.html

head -c 16 /dev/urandom | base64
来源：http://hz.aizwys.cn/gtuwnruzlq.html

[R70] 时间戳与互转
来源：http://hz.kuanghao11.cn/gtzytpizwq.html

date +%s;  date -d @1700000000
来源：http://hz.hammf.cn/gteiqcuxql.html

[R71] 日期格式化
来源：http://hz.yanxiufei.cn/gtxlkrkdeo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ydjk.org.cn/gtmsbtkeip.html

[R72] 等待端口就绪
来源：http://hz.pengpengdd.cyou/gtjmvdhhux.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yvedp.cn/gtcowtrcwh.html

[R73] 分割大日志
来源：http://hz.316326.xyz/gtbhorxfzl.html

split -l 1000 big.log part_
来源：http://hz.shanyushiyangkeji.top/gtgofliapa.html

[R74] 批量重命名
来源：http://hz.cucudq.cn/gtlpqvrvdr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jiagoushi.top/gtzygawjwb.html

[R75] 导出环境变量
来源：http://hz.hammf.cn/gtazbychaf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.c1oappe.top/gtjakgjtat.html

[R76] 使用临时文件
来源：http://hz.shanyushiyangtech.top/gtrvfwdogl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gtorslrhqg.html

[R77] 读取用户输入
来源：http://hz.gzhubu.top/gtigcezlaz.html

read -rp "请输入: " ans
来源：http://hz.jiagoushi.top/gtbukpzzar.html

[R78] 交互式菜单
来源：http://hz.yangfankeji.com/gtfzotcofm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.smart0.xyz/gtvrpxdewr.html

[R79] 解析命令行选项
来源：http://hz.zycfv.cn/gtsrcwdxrm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.fzhhl.top/gtorycktze.html

[R80] 查看脚本执行耗时
来源：http://hz.cqqwz.cn/gtqhluqhyp.html

time ./run.sh
来源：http://hz.hongshengwenyu.top/gtgdeqkhkj.html

================================================================================
来源：http://hz.yj20258.top/gtbcykgonl.html

S. C / C++ 专题
来源：http://hz.ywan-chungtsiang.top/gtyjvljtdw.html

================================================================================
来源：http://hz.daxiang520.top/gttbmeyvab.html

[S01] C：Hello World
来源：http://hz.yangfankeji.com/gtvqxbsubp.html

#include <stdio.h>
来源：http://hz.cashguo.top/gtomvluyny.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.c1oappe.top/gtsrqhaubg.html

[S02] C：变量与格式化输出
来源：http://hz.nanxuanxn.top/gtfbkujsht.html

int a = 10; printf("%d\n", a);
来源：http://hz.nwbrower.top/gtryupplvr.html

[S03] C：读入整数
来源：http://hz.ehwqpu.com/gtpjkegemf.html

int x; scanf("%d", &x);
来源：http://hz.svipenyu.cn/gtskcetiak.html

[S04] C：字符串复制
来源：http://hz.cheryme.top/gtmqyvxsdt.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zdqjudy.top/gtaophicrn.html

[S05] C：字符串长度
来源：http://hz.tianlin.xyz/gtrqcqsveq.html

strlen(s)
来源：http://hz.dashuyun.cn/gtscbzqgek.html

[S06] C：字符串比较
来源：http://hz.jinqigufen.top/gtriwgumpc.html

strcmp(a, b) == 0
来源：http://hz.fzhhl.top/gtnpkcmokw.html

[S07] C：数组遍历求和
来源：http://hz.pengpengdd.cyou/gtvslserpw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sufxvd.cn/gtyliglpum.html

[S08] C：动态内存分配与释放
来源：http://hz.zycfv.cn/gtfyqjbtdh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.sxryk.cn/gtdvdjmtwe.html

[S09] C：结构体定义与初始化
来源：http://hz.mhx1999.top/gtejkaekpv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cheryme.top/gtlfuxfelh.html

[S10] C：指针与解引用
来源：http://hz.iojbl.cn/gtgaajxwub.html

int *p = &a;  *p = 5;
来源：http://hz.guannengcc.top/gtfdktzntc.html

[S11] C：逐行读文件
来源：http://hz.shangyingyoupin.top/gtzumhqhrb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jiagoushi.top/gtqyrsjmsd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.aizwys.cn/gtzzqtmcrn.html

fclose(f);
来源：http://hz.sxryk.cn/gttmmyibmp.html

[S12] C：写文件
来源：http://hz.ydzc1.top/gtggqzbxil.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.mhx1999.top/gtvjptkimp.html

[S13] C：宏定义
来源：http://hz.shanyushiyangtech.top/gtdknnignr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shanyushiyangkeji.top/gtirkqhyhy.html

[S14] C：枚举
来源：http://hz.ppjwa.cn/gtwuzmamxh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xziqi.cn/gtcokjxanb.html

[S15] C：类型转换
来源：http://hz.tian-w.cn/gtubwnmcwz.html

(double) a / b
来源：http://hz.316326.xyz/gtspqwpnyh.html

[S16] C：位操作置位
来源：http://hz.guannengcc.top/gtlcxvlsif.html

x |= (1 << 3);
来源：http://hz.aizwys.cn/gtyrudsejh.html

[S17] C：安全拼接字符串
来源：http://hz.jinyuanbaomall.cn/gtqdgqyznn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.tianlin.xyz/gtkmwklvnm.html

[S18] C：命令行参数
来源：http://hz.zhengqikj.top/gtjgdasbsr.html


<!-- 参考信息 -->