代发 wailian999

[Q63] 开启事务
来源：http://hz.xylfe.cn/gtdeovqzrw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jianghu66.top/gttprbysjd.html

[Q64] 提交事务
来源：http://hz.feifeiyinyue.top/gtsieyjexw.html

COMMIT;
来源：http://hz.hnqzz.top/gtnzsaqjvk.html

[Q65] 回滚事务
来源：http://hz.jianghu66.top/gtrkrqrgjn.html

ROLLBACK;
来源：http://hz.zhiwuduotai.top/gtfjagqswh.html

[Q66] 行锁查询
来源：http://hz.aizwys.cn/gtrxyyduxq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xuanzx.com/gtrsvooirq.html

[Q67] 设置隔离级别
来源：http://hz.cashguo.top/gtlxqpixgh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.havefunace.top/gtkdpqaumx.html

[Q68] 保存点
来源：http://hz.9152youxi.cn/gtjfviocsc.html

SAVEPOINT sp1;
来源：http://hz.feifeiyinyue.top/gtfmmcvuey.html

ROLLBACK TO sp1;
来源：http://hz.gzhubu.top/gtleipuwlw.html

[Q69] 查看执行计划
来源：http://hz.yangfankeji.com/gtlapylpmr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.wangshuangyany.cn/gtcziigcvx.html

[Q70] 更新统计信息
来源：http://hz.jinqigufen.top/gtjykioxec.html

ANALYZE TABLE users;
来源：http://hz.hnqzz.top/gtiozsbkhj.html

[Q71] 查看建表语句
来源：http://hz.chenzaomai.com/gtemvzrjmv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinghuilouyu.cn/gtrupzzult.html

[Q72] 查看索引
来源：http://hz.meibo888.top/gtijlcypwt.html

SHOW INDEX FROM users;
来源：http://hz.zhongyouzk.top/gtjpweplqa.html

[Q73] 查看表状态
来源：http://hz.ppjwa.cn/gtasnutxfu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.chenjidiqi.icu/gtntzwtpsn.html

[Q74] 强制使用索引
来源：http://hz.52xcode.cn/gtdojvvevv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigufen.top/gtpjwjcydh.html

[Q75] 日期格式化
来源：http://hz.cdnleiting.top/gtbgahuljt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.52xcode.cn/gtqvnooizh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yueranfly.top/gtcotmdozn.html

[Q76] 按天统计
来源：http://hz.yj20258.top/gtpxgdvrtw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shanyushiyangkeji.top/gtdhuouude.html

[Q77] 时间加减
来源：http://hz.hysaishi.cn/gtvnilfigv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fengsongda.top/gttwybjahn.html

[Q78] 当前时间
来源：http://hz.xuetiantiany.cn/gtxcpvkcxy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yuanzhike.top/gtolagklnw.html

[Q79] 字符串拼接
来源：http://hz.yueranfly.top/gtvwxqhfdc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zdqjudy.top/gtlzrleeqp.html

[Q80] 字符串截取
来源：http://hz.yj202588.top/gtvrjxvoxw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.mhx1999.top/gtymoycbwp.html

[Q81] 字符串替换
来源：http://hz.hnxiangtu.top/gtcokgavzl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hywenlv.cn/gtjmrkhego.html

[Q82] 字符长度与字节长度
来源：http://hz.bjfxy.top/gthqfygtzd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtjefczwaw.html

[Q83] 大小写转换
来源：http://hz.zhixingplan.top/gtoznfgkfp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hnxiangtu.top/gtfbwpiilg.html

[Q84] 去除首尾空格
来源：http://hz.jqgfzy.top/gtyqarnnmg.html

SELECT TRIM(name) FROM users;
来源：http://hz.cqqwz.cn/gtapxxjlcq.html

[Q85] 数值取整
来源：http://hz.cashguo.top/gtimqsurgi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hywenlv.cn/gtrxizqgbd.html

[Q86] 读取 JSON 字段
来源：http://hz.yongpay.top/gttyumkogt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.havefunace.top/gtyihymzkq.html

[Q87] JSON 字段做条件
来源：http://hz.pengpengdd.cyou/gttosdhfoq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ydjk.org.cn/gtybfhzlgo.html

[Q88] 行转列（条件聚合）
来源：http://hz.yvedp.cn/gtyoxwpbrw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tanke756.top/gtsprmucyc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.dashuyun.cn/gtrnufkkcp.html

[Q89] 判断表是否存在
来源：http://hz.tianlin.xyz/gtmwyrzijn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xingfuxueyuan.xyz/gtqqnawowp.html

[Q90] 生成序号列
来源：http://hz.sysykeji.top/gtduqvpdqc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yueranfly.top/gtznnlvsyh.html

================================================================================
来源：http://hz.yangfankeji.com/gtllofzvhe.html

R. Bash 专题
来源：http://hz.jinqigufen.top/gthbtmoodz.html

================================================================================
来源：http://hz.meibo888.top/gtnqasaytu.html

[R01] shebang 与严格模式
来源：http://hz.gotoacloud.top/gtugwbnkak.html

#!/usr/bin/env bash
来源：http://hz.smart0.xyz/gtqmzzepcq.html

set -euo pipefail
来源：http://hz.chenzaomai.com/gtcpvhslkt.html

[R02] 变量赋值与使用
来源：http://hz.wangdashe.top/gtwhmdyuwn.html

name="Tom"; echo "$name"
来源：http://hz.pycfn.com/gtpnjqneib.html

[R03] 只读变量
来源：http://hz.guowangkeji.top/gtygvwrvqd.html

readonly PI=3.14
来源：http://hz.zhixingplan.top/gtsjvdsaic.html

[R04] 位置参数
来源：http://hz.pengpengdd.cyou/gtwiywppce.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ehwqpu.com/gtijffqbtj.html

[R05] 参数默认值
来源：http://hz.andypj.xyz/gtvobcwlck.html

name="${1:-default}"
来源：http://hz.fzhhl.top/gtvpekfqut.html

[R06] 判断命令是否存在
来源：http://hz.haohaochexian.top/gtfxmengqn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hnxiangtu.top/gtkdupzrah.html

[R07] if 判断文件
来源：http://hz.cqqwz.cn/gtzbrnmrvs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xinyue.icu/gtajrulrty.html

[R08] 数值比较
来源：http://hz.pycfn.com/gtsleovtvi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.andypj.xyz/gtckffvkzo.html

[R09] 字符串比较
来源：http://hz.nwbrower.top/gtztoptauh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.aizwys.cn/gtyqqvwchf.html

[R10] 正则匹配
来源：http://hz.pengpengdd.cyou/gtexeoxtyv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ybcxt.top/gtrdqnpafc.html

[R11] case 多分支
来源：http://hz.jlsjyb.cn/gtebyjtdvh.html

case "$1" in
来源：http://hz.hfpthk.cn/gtezmbmzdk.html

start) echo "启动" ;;
来源：http://hz.pycfn.com/gtdmlsonxn.html

stop)  echo "停止" ;;
来源：http://hz.andypj.xyz/gttusapizv.html

*)     echo "未知命令" ;;
来源：http://hz.snrcjt.cn/gtqdkflqli.html

esac
来源：http://hz.hnxiangtu.top/gtgmwfnwdu.html

[R12] for 遍历文件
来源：http://hz.xziqi.cn/gttfrgsomo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sufxvd.cn/gtmoaakebz.html

[R13] for 计数循环
来源：http://hz.hongshengwenyu.top/gtfcbhnylm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nwbrower.top/gtmautjuiz.html

[R14] C 风格 for
来源：http://hz.gogol.net.cn/gtaqvsokis.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shanyushiyangkeji.top/gttiidrgwq.html

[R15] while 逐行读文件
来源：http://hz.zhoulong.xyz/gtanqyjzur.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.316326.xyz/gtfissshor.html

[R16] until 等待条件
来源：http://hz.yuxming.cn/gtltsvrkfk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gotoacloud.top/gtxjigzedx.html

[R17] 数组定义与取值
来源：http://hz.cqqwz.cn/gtrzebtmdw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ydjk.org.cn/gtlseswbdp.html

[R18] 遍历数组
来源：http://hz.ehwqpu.com/gtkayskszf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.chenjidiqi.icu/gtgvzbvswm.html

[R19] 数组长度
来源：http://hz.wangdashe.top/gtaxmclgaf.html

echo "${#arr[@]}"
来源：http://hz.iojbl.cn/gtxpqnbbit.html

[R20] 关联数组（字典）
来源：http://hz.jianghu66.top/gtepseyfht.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.haohaochexian.top/gtakjveqqv.html

[R21] 字符串长度
来源：http://hz.pengpengdd.cyou/gttqaecqbv.html

echo "${#s}"
来源：http://hz.chenjidiqi.icu/gtmnpslvrn.html

[R22] 截取子串
来源：http://hz.yonumen.top/gtgsuterbk.html

echo "${s:0:5}"
来源：http://hz.gaohongyu789.top/gtiobarpxq.html

[R23] 字符串替换
来源：http://hz.ppjwa.cn/gtllnendxg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shanyushiyangtech.top/gtphmrvlsg.html

[R24] 大小写转换
来源：http://hz.yj20258.top/gtdwivvhky.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258.top/gtabstzjvo.html

[R25] 去后缀 / 去前缀
来源：http://hz.ppjwa.cn/gtakvdlkof.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yj20258888.top/gtzcssuxfd.html

[R26] 命令替换
来源：http://hz.yueranfly.top/gtjtkqzszl.html

now=$(date +%F); echo "$now"
来源：http://hz.bjfxy.top/gteyxxxvub.html

[R27] 算术展开
来源：http://hz.havefunace.top/gtttqcilrw.html

echo $((1 + 2 * 3))
来源：http://hz.guannengcc.top/gtxcfgfxbu.html

[R28] 浮点运算
来源：http://hz.jinyuanbaomall.cn/gtcfvihkji.html

echo "scale=2; 10/3" | bc
来源：http://hz.316326.xyz/gtfnaczwap.html

[R29] 定义函数
来源：http://hz.smart0.xyz/gtuqszgvjg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shzxlz.cn/gtpeyrtxoa.html

[R30] 函数返回状态码
来源：http://hz.yanxiufei.cn/gtpfbayeba.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nanxinkj.top/gtlwjslkjj.html

[R31] 局部变量
来源：http://hz.hammf.cn/gtyzkvmqdu.html

f() { local x=1; echo "$x"; }
来源：http://hz.meibo888.top/gtvjcytyxm.html

[R32] 参数个数校验
来源：http://hz.gogol.net.cn/gtjodyvgut.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.haohaochexian.top/gtkxoimonl.html

[R33] 捕获错误并提示行号
来源：http://hz.zhijiandao.cn/gtmmsumudd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.redwolf501.top/gtpunozaqh.html

[R34] 退出时清理
来源：http://hz.0kj1m.cn/gtqjmrpiwx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.bjfxy.top/gtltufegkw.html

[R35] 后台执行并等待
来源：http://hz.haohaochexian.top/gtjvhkisdx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.aibaodan.cn/gtbgvfexwz.html

[R36] 并发执行多个任务
来源：http://hz.c1oappe.top/gtnbxsewdr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zdqjudy.top/gtyblpnxcc.html

[R37] 把输出赋给变量
来源：http://hz.nanxuanxn.top/gtyxafdftl.html

files=$(ls -1)
来源：http://hz.yonumen.top/gtxqjthnoa.html

[R38] 管道串联
来源：http://hz.pycfn.com/gtnkocuyxv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgfzy.top/gtkvspfdss.html

[R39] 重定向标准输出与错误
来源：http://hz.zhijiandao.cn/gtbslqnkue.html

cmd > out.log 2>&1
来源：http://hz.shangyingyoupin.top/gtnbqjttsk.html

[R40] 追加写日志
来源：http://hz.yanxiufei.cn/gtdcynpskf.html

echo "log" >> out.log
来源：http://hz.cheryme.top/gtxrwiywwf.html

[R41] 丢弃输出
来源：http://hz.fengsongda.top/gtmfsosxll.html

cmd >/dev/null 2>&1
来源：http://hz.zhoulong.xyz/gtoojppywi.html

[R42] 输入重定向
来源：http://hz.nwbrower.top/gtwtknniau.html

wc -l < a.txt
来源：http://hz.sufxvd.cn/gtvgkmppur.html

[R43] 按名字查找文件
来源：http://hz.chenlongwang.top/gtwsnmprzc.html

find . -name "*.log" -type f
来源：http://hz.yj20258888.top/gtaygmcvxr.html

[R44] 按修改时间查找
来源：http://hz.dashuyun.cn/gtgagsjklb.html

find . -mtime -7 -type f
来源：http://hz.birdmap.top/gtnybzwypb.html

[R45] 批量删除
来源：http://hz.tian-w.cn/gtcwckmxtl.html

find . -name "*.tmp" -delete
来源：http://hz.tianlin.xyz/gtfzbnivvx.html

[R46] 递归替换文件内容
来源：http://hz.sweek.top/gtalhdimhk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hywenlv.cn/gtsvjozcpv.html

[R47] sed 单行替换
来源：http://hz.havefunace.top/gtslmunkrw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.pycfn.com/gtnuebfhes.html

[R48] awk 取指定列
来源：http://hz.sweek.top/gtnyufsawg.html

awk '{print $1, $3}' a.txt
来源：http://hz.hywenlv.cn/gtiniiiktg.html

[R49] awk 带条件
来源：http://hz.sxryk.cn/gtkqxzglra.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yongpay.top/gtqzlbftah.html

[R50] awk 求和
来源：http://hz.gzhubu.top/gtvvyuhksc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yueranfly.top/gtvkumduva.html

[R51] 排序去重取前几
来源：http://hz.jlsjyb.cn/gtritgptpb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.pengpengdd.cyou/gtqxsxknaw.html

[R52] 统计行数
来源：http://hz.shanyushiyangtech.top/gthphiatzr.html

wc -l a.txt
来源：http://hz.ywan-chungtsiang.top/gtencafmvf.html

[R53] 查看文件头与实时尾
来源：http://hz.havefunace.top/gtxalefoii.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jyoumei.cn/gtdchcashy.html

[R54] 比较两个文件
来源：http://hz.9152youxi.cn/gtqmeqbgmp.html

diff a.txt b.txt
来源：http://hz.shanyushiyangtech.top/gtmrejdmww.html

[R55] 压缩与解压
来源：http://hz.haohaochexian.top/gtxlxgctlz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jianghu66.top/gtvzchrzgp.html

[R56] 远程拷贝
来源：http://hz.nanxinkj.top/gtkydclrzc.html

scp file user@host:/path/
来源：http://hz.hysaishi.cn/gtzrfssvio.html

[R57] 远程执行命令
来源：http://hz.c1oappe.top/gtoflkpztc.html

ssh user@host 'uptime'
来源：http://hz.cheryme.top/gteoypafiz.html

[R58] 下载文件
来源：http://hz.hammf.cn/gtvjnfxrzg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gaohongyu789.top/gtsggxoscy.html

[R59] 发 POST JSON
来源：http://hz.sweek.top/gtziilhixn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.nanxinkj.top/gtdxmbrsks.html

[R60] 只看 HTTP 状态码
来源：http://hz.shzxlz.cn/gtgkxlpsku.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.snrcjt.cn/gtlouhpivy.html

[R61] 磁盘占用
来源：http://hz.yonumen.top/gtpxmcgqgt.html

df -h;  du -sh *
来源：http://hz.yonumen.top/gtdommpmmi.html

[R62] 找最占空间的文件
来源：http://hz.guannengcc.top/gttegvlaly.html

du -ah . | sort -rh | head -10
来源：http://hz.chenjidiqi.icu/gtsoenofcd.html

[R63] 内存与进程
来源：http://hz.sufxvd.cn/gtogcmrdyq.html

free -h;  ps aux | grep nginx
来源：http://hz.svipenyu.cn/gtvteyepyb.html

[R64] 结束进程
来源：http://hz.yj202588.top/gtvlcdhfea.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gogol.net.cn/gttddjtjbt.html

[R65] 查看端口占用
来源：http://hz.hnqzz.top/gtnjoghjhq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ppjwa.cn/gtrhrobjct.html

[R66] 定时任务
来源：http://hz.aizwys.cn/gtibtyjtte.html

crontab -e;  crontab -l
来源：http://hz.guowangkeji.top/gtlpmpqogx.html

[R67] 生成随机十六进制串
来源：http://hz.gogol.net.cn/gthzhihwrh.html

openssl rand -hex 16
来源：http://hz.havefunace.top/gtctflefpy.html

[R68] 计算文件校验值
来源：http://hz.bjfxy.top/gtclunssqr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.mhx1999.top/gtsxjptoxl.html

[R69] 生成随机密码
来源：http://hz.wangshuangyany.cn/gtwnytmpdl.html

head -c 16 /dev/urandom | base64
来源：http://hz.nwbrower.top/gtufqyvzwa.html

[R70] 时间戳与互转
来源：http://hz.gaohongyu789.top/gtmokgsnvx.html

date +%s;  date -d @1700000000
来源：http://hz.meibo888.top/gteetkijgr.html

[R71] 日期格式化
来源：http://hz.hammf.cn/gtclrpazdx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinyuanbaomall.cn/gtxlpgkxcw.html

[R72] 等待端口就绪
来源：http://hz.sufxvd.cn/gttjqlbsoe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydzc1.top/gtpmolrqil.html

[R73] 分割大日志
来源：http://hz.havefunace.top/gtbaitvnnj.html

split -l 1000 big.log part_
来源：http://hz.svipenyu.cn/gtcvtkkofo.html

[R74] 批量重命名
来源：http://hz.yuanzhike.top/gttvnnkwlt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.c1oappe.top/gtwoqdhfgn.html

[R75] 导出环境变量
来源：http://hz.havefunace.top/gtgvrgkavr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.iojbl.cn/gtqjccevey.html

[R76] 使用临时文件
来源：http://hz.pycfn.com/gtrorttwcz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zycfv.cn/gttflsxavw.html

[R77] 读取用户输入
来源：http://hz.jianghu66.top/gtxpwucikf.html

read -rp "请输入: " ans
来源：http://hz.iojbl.cn/gtltdtkode.html

[R78] 交互式菜单
来源：http://hz.jyoumei.cn/gthfbqmpqb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nanxuanxn.top/gtgeevepse.html

[R79] 解析命令行选项
来源：http://hz.9152youxi.cn/gtlvyfnpjv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tian-w.cn/gtqpstiwxp.html

[R80] 查看脚本执行耗时
来源：http://hz.hnxiangtu.top/gtofnmwjoh.html

time ./run.sh
来源：http://hz.ehwqpu.com/gtogzqujbr.html

================================================================================
来源：http://hz.chenjidiqi.icu/gthmmzalyg.html

S. C / C++ 专题
来源：http://hz.ydjk.org.cn/gtpifnqoyy.html

================================================================================
来源：http://hz.ivvv.top/gtwlghfhic.html

[S01] C：Hello World
来源：http://hz.cucudq.cn/gtiionzads.html

#include <stdio.h>
来源：http://hz.shanyushiyangtech.top/gtkksqqujp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cdnleiting.top/gtungtbtmi.html

[S02] C：变量与格式化输出
来源：http://hz.jqgufenzy.top/gtlmirheef.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenjidiqi.icu/gtezkaoloi.html

[S03] C：读入整数
来源：http://hz.jinqigufen.top/gtsdcuyscv.html

int x; scanf("%d", &x);
来源：http://hz.yj202588.top/gttiancjhv.html

[S04] C：字符串复制
来源：http://hz.shuidangran.top/gtuaorfdtf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhijiandao.cn/gtohfbrkct.html

[S05] C：字符串长度
来源：http://hz.hnxiangtu.top/gtdlielktq.html

strlen(s)
来源：http://hz.gogol.net.cn/gtiszjmqst.html

[S06] C：字符串比较
来源：http://hz.316326.xyz/gtplsnbziq.html

strcmp(a, b) == 0
来源：http://hz.hnxiangtu.top/gtmuplnhnl.html

[S07] C：数组遍历求和
来源：http://hz.bjfxy.top/gtjxrispui.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tanke756.top/gtdsmxrjwk.html

[S08] C：动态内存分配与释放
来源：http://hz.xuanzx.com/gtnvmoffqs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.wangshuangyany.cn/gtfjuiymxy.html

[S09] C：结构体定义与初始化
来源：http://hz.svipenyu.cn/gtzrosxeck.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hfpthk.cn/gtspyxwfxq.html

[S10] C：指针与解引用
来源：http://hz.quarkkingdee.top/gteaxfypqb.html

int *p = &a;  *p = 5;
来源：http://hz.gaohongyu789.top/gtctpshmca.html

[S11] C：逐行读文件
来源：http://hz.chenzaomai.com/gtcckivbgg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhiwuduotai.top/gtvpjjilyr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxuanxn.top/gtkmbfxsmk.html

fclose(f);
来源：http://hz.jinqigufen.top/gtdvygtvfh.html

[S12] C：写文件
来源：http://hz.hywenlv.cn/gtzqltplcs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.guannengcc.top/gttaeebrho.html

[S13] C：宏定义
来源：http://hz.jianghu66.top/gtzloepkpz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xziqi.cn/gtunavxkut.html

[S14] C：枚举
来源：http://hz.jinyuanbaomall.cn/gtvgpfooxd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cdnleiting.top/gtcrhnhpvf.html

[S15] C：类型转换
来源：http://hz.hnxiangtu.top/gtuwgqkcxs.html

(double) a / b
来源：http://hz.tianlin.xyz/gtksatdqjf.html

[S16] C：位操作置位
来源：http://hz.yj202588.top/gtddnemrvw.html

x |= (1 << 3);
来源：http://hz.nanxuanxn.top/gthllzefap.html

[S17] C：安全拼接字符串
来源：http://hz.cheryme.top/gtsgfrtthb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gotoacloud.top/gtgvbeycjz.html

[S18] C：命令行参数
来源：http://hz.cashguo.top/gtzfdzslyb.html

int main(int argc, char **argv)
来源：http://hz.gotoacloud.top/gtcmobmgnn.html

[S19] C：快速排序
来源：http://hz.jiagoushi.top/gtsidppmil.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gtgojhbcvq.html

[S20] C：二分查找
来源：http://hz.zycfv.cn/gtvwfjtuje.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhijiandao.cn/gtmwddkxng.html

[S21] C：字符类别判断
来源：http://hz.jqgfzy.top/gtjugplhmf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gotoacloud.top/gtewlrphcl.html

[S22] C：字符串转数字
来源：http://hz.tian-w.cn/gtceupylgq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xziqi.cn/gtcqkprblu.html

[S23] C：随机数
来源：http://hz.hongshengwenyu.top/gtyhzctiwx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.dianchejie.cn/gtywnerkus.html

[S24] C：获取本地时间
来源：http://hz.hysaishi.cn/gtdrympeyd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ybcxt.top/gtupzunkdc.html

[S25] C：内存拷贝
来源：http://hz.316326.xyz/gtaygjvghw.html

memcpy(dst, src, n);
来源：http://hz.yvedp.cn/gtidiivzyt.html

[S26] C：内存清零
来源：http://hz.vqdsnc.cn/gtnugxvsiz.html

memset(a, 0, sizeof a);
来源：http://hz.jqgufenzy.top/gtajgwpcdq.html

[S27] C：定义常量
来源：http://hz.zhaomingkeji.xyz/gtqlzfhgmv.html

const double PI = 3.14159;
来源：http://hz.xuanzx.com/gtydygdbrk.html

[S28] C：静态变量
来源：http://hz.xingfuxueyuan.xyz/gthllhqiag.html

static int counter = 0;
来源：http://hz.yangfankeji.com/gtkzopcixo.html

[S29] C：变参函数
来源：http://hz.chenjidiqi.icu/gtmvbytqhw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hongshengwenyu.top/gtsowmrtsi.html

[S30] C：头文件保护
来源：http://hz.quarkkingdee.top/gtgoqtinuw.html

#ifndef X_H
来源：http://hz.hnqzz.top/gtqnllhmow.html

#define X_H
来源：http://hz.hammf.cn/gtggcfybfe.html

#endif
来源：http://hz.xinyue.icu/gtijadogem.html

[S31] C++：Hello World
来源：http://hz.hnxiangtu.top/gtwwjivfgk.html

#include <iostream>
来源：http://hz.0kj1m.cn/gtkbdpazdf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yonumen.top/gtwurjmebj.html

[S32] C++：字符串
来源：http://hz.dianchejie.cn/gtdfdakrxj.html

std::string s = "hi";  s += "!";
来源：http://hz.shanyushiyangtech.top/gtlnumvzau.html


<!-- 参考信息 -->