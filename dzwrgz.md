代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.bjfxy.top/gtxzgblcyb.html

[Q54] 清空表
来源：http://hz.xinyue.icu/gtvgmfbcmq.html

TRUNCATE TABLE logs;
来源：http://hz.jyoumei.cn/gtvvhpwgnm.html

[Q55] 排名（并列占位）
来源：http://hz.gotoacloud.top/gtjesezimv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yueranfly.top/gtmotlmwvt.html

[Q56] 密集排名（并列不占位）
来源：http://hz.kuanghao11.cn/gtoqpceamp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hywenlv.cn/gtbdtoiejo.html

[Q57] 行号
来源：http://hz.xingfuxueyuan.xyz/gtshvjlvqh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.9152youxi.cn/gtpvvhwmds.html

[Q58] 累计求和
来源：http://hz.yj20258888.top/gtynncufeu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jlsjyb.cn/gtjwmjzgmv.html

[Q59] 分组内累计
来源：http://hz.jinqigufen.top/gtzatglefz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hammf.cn/gtfnjscuhi.html

[Q60] 取上一行 / 下一行
来源：http://hz.hywenlv.cn/gtwdqwdkjx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jlsjyb.cn/gtatkvgndy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinghuilouyu.cn/gtnoijdido.html

[Q61] 移动平均
来源：http://hz.52xcode.cn/gtegikmswk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.wangshuangyany.cn/gtgjysdhfl.html

[Q62] 分组占比
来源：http://hz.gaohongyu789.top/gtiubneiut.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gthotpzkow.html

[Q63] 开启事务
来源：http://hz.c1oappe.top/gtfjgdffaz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhengqikj.top/gtctsydfsr.html

[Q64] 提交事务
来源：http://hz.mhx1999.top/gteccmvzna.html

COMMIT;
来源：http://hz.hongshengwenyu.top/gttqutxwbb.html

[Q65] 回滚事务
来源：http://hz.zhongyouzk.top/gtopdnwtdf.html

ROLLBACK;
来源：http://hz.jinyuanbaomall.cn/gtxbxluoae.html

[Q66] 行锁查询
来源：http://hz.shanyushiyangkeji.top/gttkzyaego.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gaohongyu789.top/gtbwjjvdou.html

[Q67] 设置隔离级别
来源：http://hz.ivvv.top/gtzuckrzjc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ywan-chungtsiang.top/gtjwambsja.html

[Q68] 保存点
来源：http://hz.shuidangran.top/gtqaicaxid.html

SAVEPOINT sp1;
来源：http://hz.birdmap.top/gtlrpmjmze.html

ROLLBACK TO sp1;
来源：http://hz.yuanzhike.top/gtwiivcxoc.html

[Q69] 查看执行计划
来源：http://hz.gogol.net.cn/gtypphwsrp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jlsjyb.cn/gtokijorum.html

[Q70] 更新统计信息
来源：http://hz.hywenlv.cn/gttwuxusqq.html

ANALYZE TABLE users;
来源：http://hz.shzxlz.cn/gtfqnrxghu.html

[Q71] 查看建表语句
来源：http://hz.feifeiyinyue.top/gthdytnaoc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.fengsongda.top/gtvjkaawca.html

[Q72] 查看索引
来源：http://hz.cashguo.top/gtyysfyuye.html

SHOW INDEX FROM users;
来源：http://hz.tianlin.xyz/gtwqdejezf.html

[Q73] 查看表状态
来源：http://hz.shanyushiyangtech.top/gtymebbxdr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.guowangkeji.top/gtwouksmec.html

[Q74] 强制使用索引
来源：http://hz.cucudq.cn/gtkpvcixpw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.pengpengdd.cyou/gtimozpksn.html

[Q75] 日期格式化
来源：http://hz.xingfuxueyuan.xyz/gtemsashij.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenlongwang.top/gthdmconbs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yj20258888.top/gtwjqzmxpg.html

[Q76] 按天统计
来源：http://hz.zhiwuduotai.top/gtzkhkplwa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hammf.cn/gtxhfvhrgo.html

[Q77] 时间加减
来源：http://hz.cqqwz.cn/gtlgfokciw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gaohongyu789.top/gtiuihjsns.html

[Q78] 当前时间
来源：http://hz.bjfxy.top/gtxsxbdrlo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nanxuanxn.top/gtwhfacqer.html

[Q79] 字符串拼接
来源：http://hz.chenlongwang.top/gtookahlgl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xuanzx.com/gtdjpsssgr.html

[Q80] 字符串截取
来源：http://hz.vqdsnc.cn/gtqwwesgog.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ydzc1.top/gtnhjmzzip.html

[Q81] 字符串替换
来源：http://hz.chenjidiqi.icu/gtoeejfceo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hongshengwenyu.top/gtzipuinva.html

[Q82] 字符长度与字节长度
来源：http://hz.shanyushiyangkeji.top/gtkkusjizh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ydzc1.top/gtwrdloavs.html

[Q83] 大小写转换
来源：http://hz.aibaodan.cn/gtmdszvdzu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cqqwz.cn/gtwgwgekvf.html

[Q84] 去除首尾空格
来源：http://hz.haohaochexian.top/gtbkmlijsf.html

SELECT TRIM(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtvglueevl.html

[Q85] 数值取整
来源：http://hz.zhaomingkeji.xyz/gtdxnuzpue.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.sweek.top/gtwvlhrmil.html

[Q86] 读取 JSON 字段
来源：http://hz.hywenlv.cn/gtzvvmzvmh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hnqzz.top/gtbrvqkavi.html

[Q87] JSON 字段做条件
来源：http://hz.c1oappe.top/gtjjaowrif.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhixingplan.top/gtdfcposnw.html

[Q88] 行转列（条件聚合）
来源：http://hz.hfpthk.cn/gtgkhdilzy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.haohaochexian.top/gthjllmpew.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.smart0.xyz/gtmnaismdg.html

[Q89] 判断表是否存在
来源：http://hz.mhx1999.top/gtspubknxp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hongshengwenyu.top/gtgwssqxbh.html

[Q90] 生成序号列
来源：http://hz.zycfv.cn/gtravsupzv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ydzc1.top/gtmnoytwlj.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtwuqeaiyf.html

R. Bash 专题
来源：http://hz.yangfankeji.com/gtrhkgknqe.html

================================================================================
来源：http://hz.gaohongyu789.top/gtqeowniic.html

[R01] shebang 与严格模式
来源：http://hz.guannengcc.top/gtgrgkxnan.html

#!/usr/bin/env bash
来源：http://hz.daria6918.cn/gtnszwblnv.html

set -euo pipefail
来源：http://hz.yanxiufei.cn/gtmduznizr.html

[R02] 变量赋值与使用
来源：http://hz.meibo888.top/gtflsaztot.html

name="Tom"; echo "$name"
来源：http://hz.zhaomingkeji.xyz/gtpuhdfiwc.html

[R03] 只读变量
来源：http://hz.gotoacloud.top/gtciwjxhxk.html

readonly PI=3.14
来源：http://hz.redwolf501.top/gtppbofbyg.html

[R04] 位置参数
来源：http://hz.ywan-chungtsiang.top/gttxxoques.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sufxvd.cn/gtyrefymxo.html

[R05] 参数默认值
来源：http://hz.andypj.xyz/gtkmhfakwb.html

name="${1:-default}"
来源：http://hz.feifeiyinyue.top/gthghbxrzm.html

[R06] 判断命令是否存在
来源：http://hz.zdqjudy.top/gterlyfpnf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hongshengwenyu.top/gtuhfgrvme.html

[R07] if 判断文件
来源：http://hz.xuetiantiany.cn/gtwkpwwyiw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ywan-chungtsiang.top/gtojeplpck.html

[R08] 数值比较
来源：http://hz.iojbl.cn/gtnxhwxhfh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.aibaodan.cn/gtmkshcaxz.html

[R09] 字符串比较
来源：http://hz.xuetiantiany.cn/gtgezvdzqc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.quarkkingdee.top/gtyxdvxvqx.html

[R10] 正则匹配
来源：http://hz.andypj.xyz/gtzlntqwci.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinghuilouyu.cn/gtjklaidcl.html

[R11] case 多分支
来源：http://hz.zhiwuduotai.top/gtkaryvnbu.html

case "$1" in
来源：http://hz.haohaochexian.top/gtsldgrvjn.html

start) echo "启动" ;;
来源：http://hz.vqdsnc.cn/gtavlrzage.html

stop)  echo "停止" ;;
来源：http://hz.zhixingplan.top/gtroxkyznc.html

*)     echo "未知命令" ;;
来源：http://hz.cqqwz.cn/gtbnnkztmg.html

esac
来源：http://hz.pycfn.com/gthniesbcq.html

[R12] for 遍历文件
来源：http://hz.jqgfzy.top/gtyxbkhcfu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jianghu66.top/gtpzmnwgjr.html

[R13] for 计数循环
来源：http://hz.yonumen.top/gtnovriyuo.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.aibaodan.cn/gtkcayphdi.html

[R14] C 风格 for
来源：http://hz.shzxlz.cn/gtcudmhlau.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hfpthk.cn/gtvxuftoic.html

[R15] while 逐行读文件
来源：http://hz.sysykeji.top/gtkgpcwsaq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jlsjyb.cn/gtfgyjdcot.html

[R16] until 等待条件
来源：http://hz.pengpengdd.cyou/gtvfjidkfd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.mhx1999.top/gtbmgzmamw.html

[R17] 数组定义与取值
来源：http://hz.yanxiufei.cn/gtgqistynd.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.wangshuangyany.cn/gtvsnuincp.html

[R18] 遍历数组
来源：http://hz.fzhhl.top/gtvmjwelnm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cqqwz.cn/gtcwapoiya.html

[R19] 数组长度
来源：http://hz.guowangkeji.top/gtnghhpuqs.html

echo "${#arr[@]}"
来源：http://hz.sweek.top/gtbxvywdgz.html

[R20] 关联数组（字典）
来源：http://hz.yuanzhike.top/gtzkgnxskg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sysykeji.top/gtfyqgtkwq.html

[R21] 字符串长度
来源：http://hz.redwolf501.top/gtivvrugdr.html

echo "${#s}"
来源：http://hz.nanxinkj.top/gtrardidrh.html

[R22] 截取子串
来源：http://hz.yvedp.cn/gtdzxxmvaw.html

echo "${s:0:5}"
来源：http://hz.cheryme.top/gtfairfywf.html

[R23] 字符串替换
来源：http://hz.316326.xyz/gttzybprlv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jyoumei.cn/gtdbqjfxwn.html

[R24] 大小写转换
来源：http://hz.jyoumei.cn/gtfmiaargc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yvedp.cn/gtriugttyy.html

[R25] 去后缀 / 去前缀
来源：http://hz.jqgfzy.top/gtuwvkbptq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.feifeiyinyue.top/gtwocwwkkc.html

[R26] 命令替换
来源：http://hz.c1oappe.top/gtajogvvbb.html

now=$(date +%F); echo "$now"
来源：http://hz.sweek.top/gtqbuunbhf.html

[R27] 算术展开
来源：http://hz.wangshuangyany.cn/gtlhhxmsyj.html

echo $((1 + 2 * 3))
来源：http://hz.andypj.xyz/gtffyozuix.html

[R28] 浮点运算
来源：http://hz.jyoumei.cn/gtcjibjacz.html

echo "scale=2; 10/3" | bc
来源：http://hz.jlsjyb.cn/gthrtezgcc.html

[R29] 定义函数
来源：http://hz.sysykeji.top/gtzzysfypm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guannengcc.top/gtinaircoe.html

[R30] 函数返回状态码
来源：http://hz.zhongyouzk.top/gtcwrqqnpd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ydzc1.top/gtovppkyjm.html

[R31] 局部变量
来源：http://hz.shanyushiyangkeji.top/gtwrmitbae.html

f() { local x=1; echo "$x"; }
来源：http://hz.c1oappe.top/gtciadpbkp.html

[R32] 参数个数校验
来源：http://hz.yj20258888.top/gtrantokyg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hnxiangtu.top/gtsxsfinay.html

[R33] 捕获错误并提示行号
来源：http://hz.jinghuilouyu.cn/gtcymkogra.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.316326.xyz/gtxqlkelsi.html

[R34] 退出时清理
来源：http://hz.zhongyouzk.top/gtunvkyfed.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yueranfly.top/gtamloyesm.html

[R35] 后台执行并等待
来源：http://hz.shuidangran.top/gtvueriveo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ydzc1.top/gtmiijshgm.html

[R36] 并发执行多个任务
来源：http://hz.vqdsnc.cn/gttkbcqgcq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cashguo.top/gtqsltmqmr.html

[R37] 把输出赋给变量
来源：http://hz.yuxming.cn/gtgkeeoxki.html

files=$(ls -1)
来源：http://hz.gzhubu.top/gtijqmcwec.html

[R38] 管道串联
来源：http://hz.gotoacloud.top/gtvvetngui.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tanke756.top/gttahemiof.html

[R39] 重定向标准输出与错误
来源：http://hz.chenlongwang.top/gtpgtuhcon.html

cmd > out.log 2>&1
来源：http://hz.jqgfzy.top/gtuebbnkpi.html

[R40] 追加写日志
来源：http://hz.sweek.top/gtounhnqkl.html

echo "log" >> out.log
来源：http://hz.gaohongyu789.top/gtrzxdiwsw.html

[R41] 丢弃输出
来源：http://hz.shanyushiyangkeji.top/gtbmcauidg.html

cmd >/dev/null 2>&1
来源：http://hz.daxiang520.top/gtnsgvmlhz.html

[R42] 输入重定向
来源：http://hz.haohaochexian.top/gtnynjrfok.html

wc -l < a.txt
来源：http://hz.gogol.net.cn/gtvqudgpwr.html

[R43] 按名字查找文件
来源：http://hz.daxiang520.top/gtgephwigz.html

find . -name "*.log" -type f
来源：http://hz.zycfv.cn/gtwbgnruef.html

[R44] 按修改时间查找
来源：http://hz.dianchejie.cn/gtiftulvaw.html

find . -mtime -7 -type f
来源：http://hz.jinghuilouyu.cn/gtldzuifhx.html

[R45] 批量删除
来源：http://hz.sysykeji.top/gtlrvirviu.html

find . -name "*.tmp" -delete
来源：http://hz.jlsjyb.cn/gtpcknjrsr.html

[R46] 递归替换文件内容
来源：http://hz.nanxinkj.top/gtjtbabsao.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xylfe.cn/gtdbfmezoc.html

[R47] sed 单行替换
来源：http://hz.sweek.top/gtfpmlzqoe.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.quarkkingdee.top/gtqzttqmem.html

[R48] awk 取指定列
来源：http://hz.shanyushiyangkeji.top/gtomytbwzd.html

awk '{print $1, $3}' a.txt
来源：http://hz.tian-w.cn/gtgbozgvzh.html

[R49] awk 带条件
来源：http://hz.c1oappe.top/gtmxtyskwf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jqgufenzy.top/gtfdorrrlv.html

[R50] awk 求和
来源：http://hz.meibo888.top/gtlocgkclj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.snrcjt.cn/gtyzeotaro.html

[R51] 排序去重取前几
来源：http://hz.c1oappe.top/gtnnymvlho.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gaohongyu789.top/gtjctlnpfo.html

[R52] 统计行数
来源：http://hz.yj20258.top/gttshqhcge.html

wc -l a.txt
来源：http://hz.feifeiyinyue.top/gtbrtxyzcm.html

[R53] 查看文件头与实时尾
来源：http://hz.yonumen.top/gtuyzkziku.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dianchejie.cn/gtdmvaclxx.html

[R54] 比较两个文件
来源：http://hz.xziqi.cn/gtzyenkwqj.html

diff a.txt b.txt
来源：http://hz.kuanghao11.cn/gtnsxulkug.html

[R55] 压缩与解压
来源：http://hz.jqgufenzy.top/gtsggzphbr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.quarkkingdee.top/gtzphkzxvc.html

[R56] 远程拷贝
来源：http://hz.yj20258.top/gtlqvezztt.html

scp file user@host:/path/
来源：http://hz.hnxiangtu.top/gtpvhfkdul.html

[R57] 远程执行命令
来源：http://hz.ivvv.top/gtuauxrpyo.html

ssh user@host 'uptime'
来源：http://hz.andypj.xyz/gtyobddatv.html

[R58] 下载文件
来源：http://hz.xinyue.icu/gtgdohdsdo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.svipenyu.cn/gttilbnqct.html

[R59] 发 POST JSON
来源：http://hz.jinqigufen.top/gtufhisjke.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jianghu66.top/gtypswupwv.html

[R60] 只看 HTTP 状态码
来源：http://hz.tanke756.top/gtmsenoije.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.pengpengdd.cyou/gtjkvxdciq.html

[R61] 磁盘占用
来源：http://hz.snrcjt.cn/gtngircpmt.html

df -h;  du -sh *
来源：http://hz.yuanzhike.top/gtncdnkocy.html

[R62] 找最占空间的文件
来源：http://hz.ppjwa.cn/gtsvwwecsd.html

du -ah . | sort -rh | head -10
来源：http://hz.cdnleiting.top/gtcdzypenk.html

[R63] 内存与进程
来源：http://hz.aizwys.cn/gthntvsbta.html

free -h;  ps aux | grep nginx
来源：http://hz.xinyue.icu/gtehayvetq.html

[R64] 结束进程
来源：http://hz.yj20258888.top/gtvfzogqok.html

kill -9 $(pgrep -f app.py)
来源：http://hz.fzhhl.top/gttohwozts.html

[R65] 查看端口占用
来源：http://hz.svipenyu.cn/gtbzmhsxcu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhaomingkeji.xyz/gttmokmtsq.html

[R66] 定时任务
来源：http://hz.0kj1m.cn/gtmeqoculf.html

crontab -e;  crontab -l
来源：http://hz.jinghuilouyu.cn/gtnqfzxvyx.html

[R67] 生成随机十六进制串
来源：http://hz.cqqwz.cn/gtpndbqehg.html

openssl rand -hex 16
来源：http://hz.jqgfzy.top/gtxnjegwvr.html

[R68] 计算文件校验值
来源：http://hz.sysykeji.top/gtmgdqtqwo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yongpay.top/gtbrioqguq.html

[R69] 生成随机密码
来源：http://hz.c1oappe.top/gtxneqofzn.html

head -c 16 /dev/urandom | base64
来源：http://hz.hysaishi.cn/gtcdeyajap.html

[R70] 时间戳与互转
来源：http://hz.hongshengwenyu.top/gtktlsmikh.html

date +%s;  date -d @1700000000
来源：http://hz.feifeiyinyue.top/gteetqzhrg.html

[R71] 日期格式化
来源：http://hz.nanxuanxn.top/gtlopglxjy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xuanzx.com/gtzobpojgw.html

[R72] 等待端口就绪
来源：http://hz.9152youxi.cn/gtqlpbuuhp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hysaishi.cn/gtjkudogny.html

[R73] 分割大日志
来源：http://hz.shanyushiyangkeji.top/gtlgscqnwr.html

split -l 1000 big.log part_
来源：http://hz.dashuyun.cn/gtparpjhcl.html

[R74] 批量重命名
来源：http://hz.bjfxy.top/gtyzlyaypy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.fzhhl.top/gtirmtwvcx.html

[R75] 导出环境变量
来源：http://hz.jinqigufen.top/gtqyieopnq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hywenlv.cn/gtkgboylri.html

[R76] 使用临时文件
来源：http://hz.zhongyouzk.top/gtdcfvjmyc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhaomingkeji.xyz/gtdecqsccl.html

[R77] 读取用户输入
来源：http://hz.jqgfzy.top/gtyvxrfgnq.html

read -rp "请输入: " ans
来源：http://hz.hammf.cn/gtmgaiemfx.html

[R78] 交互式菜单
来源：http://hz.andypj.xyz/gtikdqdgor.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yvedp.cn/gthdiuscwr.html

[R79] 解析命令行选项
来源：http://hz.quarkkingdee.top/gtenumiqeh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ywan-chungtsiang.top/gtnunbhesu.html

[R80] 查看脚本执行耗时
来源：http://hz.hywenlv.cn/gtkketnxnb.html

time ./run.sh
来源：http://hz.0kj1m.cn/gtgaqxqzjq.html

================================================================================
来源：http://hz.zhongyouzk.top/gtmnphwcwm.html

S. C / C++ 专题
来源：http://hz.andypj.xyz/gtzgoqutyc.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtbbrerdhs.html

[S01] C：Hello World
来源：http://hz.wangshuangyany.cn/gtbwdaqovs.html

#include <stdio.h>
来源：http://hz.zhixingplan.top/gtjgztddpn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cashguo.top/gtrbistwtl.html

[S02] C：变量与格式化输出
来源：http://hz.birdmap.top/gtsgklctvb.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenjidiqi.icu/gtlcpavjbr.html

[S03] C：读入整数
来源：http://hz.hysaishi.cn/gtbzndduuf.html

int x; scanf("%d", &x);
来源：http://hz.zhoulong.xyz/gtgowoslkt.html

[S04] C：字符串复制
来源：http://hz.hysaishi.cn/gtoyilvgrn.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jiagoushi.top/gtbgurhnsm.html

[S05] C：字符串长度
来源：http://hz.aibaodan.cn/gthnykvdxm.html

strlen(s)
来源：http://hz.cdnleiting.top/gtveozfrbf.html

[S06] C：字符串比较
来源：http://hz.jinqigufen.top/gthspddwmw.html

strcmp(a, b) == 0
来源：http://hz.gaohongyu789.top/gtxxcuawha.html

[S07] C：数组遍历求和
来源：http://hz.guannengcc.top/gtiupdhtzu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hnqzz.top/gtmsawmjog.html

[S08] C：动态内存分配与释放
来源：http://hz.jinghuilouyu.cn/gttigclpvh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hywenlv.cn/gttjvlplhs.html

[S09] C：结构体定义与初始化
来源：http://hz.gaohongyu789.top/gtosqiuoiy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jinghuilouyu.cn/gtgssznjuo.html

[S10] C：指针与解引用
来源：http://hz.cucudq.cn/gtnwtkggqf.html

int *p = &a;  *p = 5;
来源：http://hz.ivvv.top/gttgnzpxfd.html

[S11] C：逐行读文件
来源：http://hz.gogol.net.cn/gtrnumvjcx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.iojbl.cn/gtnqgnfbvv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhongyouzk.top/gtsbhrnybi.html

fclose(f);
来源：http://hz.cqqwz.cn/gtvodykjeu.html

[S12] C：写文件
来源：http://hz.wangdashe.top/gtwzophcik.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.redwolf501.top/gthvgbenii.html

[S13] C：宏定义
来源：http://hz.hfpthk.cn/gtjutjyozi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tanke756.top/gtazpaziqh.html

[S14] C：枚举
来源：http://hz.hysaishi.cn/gtlyukryix.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gaohongyu789.top/gtocnxxxhl.html

[S15] C：类型转换
来源：http://hz.yj20258.top/gtdksuydom.html

(double) a / b
来源：http://hz.cashguo.top/gtumddwvtm.html

[S16] C：位操作置位
来源：http://hz.quarkkingdee.top/gtvpatlwuu.html

x |= (1 << 3);
来源：http://hz.haohaochexian.top/gtnjncmcce.html

[S17] C：安全拼接字符串
来源：http://hz.bjfxy.top/gtvuvtbhop.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.smart0.xyz/gtzlyexuzn.html

[S18] C：命令行参数
来源：http://hz.zdqjudy.top/gtpylktcmi.html

int main(int argc, char **argv)
来源：http://hz.zhiwuduotai.top/gtznhhmznb.html

[S19] C：快速排序
来源：http://hz.tanke756.top/gtnidkavuv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinqigfzy.top/gtcmamxkpm.html

[S20] C：二分查找
来源：http://hz.pengpengdd.cyou/gtklcqurbk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cqqwz.cn/gttirwwxsk.html

[S21] C：字符类别判断
来源：http://hz.ydjk.org.cn/gtkmqotaqt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jyoumei.cn/gtdgskiipj.html

[S22] C：字符串转数字
来源：http://hz.xuanzx.com/gthvoooevy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.kuanghao11.cn/gtqkjqwscd.html

[S23] C：随机数
来源：http://hz.zhiwuduotai.top/gtsmupkkbq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.fzhhl.top/gtmrcayguf.html

[S24] C：获取本地时间
来源：http://hz.yanxiufei.cn/gtwokpvzpm.html


<!-- 参考信息 -->