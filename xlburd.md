代发 wailian999

[Q65] 回滚事务
来源：http://hz.sxryk.cn/gtllspvnxh.html

ROLLBACK;
来源：http://hz.pycfn.com/gtguroabii.html

[Q66] 行锁查询
来源：http://hz.yuxming.cn/gtaldsribo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenjidiqi.icu/gtdrjoqeyn.html

[Q67] 设置隔离级别
来源：http://hz.zhengqikj.top/gtwjvjljwn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhiwuduotai.top/gtnyzftjyw.html

[Q68] 保存点
来源：http://hz.cucudq.cn/gtcnzbdvpz.html

SAVEPOINT sp1;
来源：http://hz.vqdsnc.cn/gtpgbhvxma.html

ROLLBACK TO sp1;
来源：http://hz.wangshuangyany.cn/gtwoytvvlj.html

[Q69] 查看执行计划
来源：http://hz.shanyushiyangkeji.top/gttchskcyr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ywan-chungtsiang.top/gtfcsnsywj.html

[Q70] 更新统计信息
来源：http://hz.jinghuilouyu.cn/gtxuqsuawt.html

ANALYZE TABLE users;
来源：http://hz.yuanzhike.top/gtshpcmniz.html

[Q71] 查看建表语句
来源：http://hz.guowangkeji.top/gtuvphvcit.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cashguo.top/gttnyddydz.html

[Q72] 查看索引
来源：http://hz.smart0.xyz/gtiedchtjd.html

SHOW INDEX FROM users;
来源：http://hz.guannengcc.top/gtssxshvky.html

[Q73] 查看表状态
来源：http://hz.cheryme.top/gtzonvhqdf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj202588.top/gtfcyhteti.html

[Q74] 强制使用索引
来源：http://hz.zhaomingkeji.xyz/gtptrounqb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.daria6918.cn/gtivyddwbi.html

[Q75] 日期格式化
来源：http://hz.redwolf501.top/gtdrmlsbuk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gogol.net.cn/gttndfvkuy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.wangshuangyany.cn/gtpsanlhrr.html

[Q76] 按天统计
来源：http://hz.chenlongwang.top/gtkabrwjlx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.pengpengdd.cyou/gthnyoenvs.html

[Q77] 时间加减
来源：http://hz.ydzc1.top/gtupyoqgcj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.daxiang520.top/gtwuepzsvb.html

[Q78] 当前时间
来源：http://hz.zhongyouzk.top/gtszaukxdr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ywan-chungtsiang.top/gtbwjoyqzr.html

[Q79] 字符串拼接
来源：http://hz.jlsjyb.cn/gtvewkjiiu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj202588.top/gtynabokcl.html

[Q80] 字符串截取
来源：http://hz.tanke756.top/gtphxocpvd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhiwuduotai.top/gtlhexphut.html

[Q81] 字符串替换
来源：http://hz.cdnleiting.top/gtskdbrpjs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.birdmap.top/gthzcgrfrj.html

[Q82] 字符长度与字节长度
来源：http://hz.daxiang520.top/gtcqtvpuza.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtevulcegz.html

[Q83] 大小写转换
来源：http://hz.zhongyouzk.top/gtpyajwgff.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.pycfn.com/gtiuboyufc.html

[Q84] 去除首尾空格
来源：http://hz.hnxiangtu.top/gtsqdnattt.html

SELECT TRIM(name) FROM users;
来源：http://hz.smart0.xyz/gtzbkqyrfl.html

[Q85] 数值取整
来源：http://hz.ehwqpu.com/gtgnxhhyqb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shanyushiyangkeji.top/gtxdnglvsu.html

[Q86] 读取 JSON 字段
来源：http://hz.hammf.cn/gtkjxgpcms.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenzaomai.com/gtlhbltrtr.html

[Q87] JSON 字段做条件
来源：http://hz.smart0.xyz/gthntlulbb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sufxvd.cn/gtgdgfzihz.html

[Q88] 行转列（条件聚合）
来源：http://hz.gaohongyu789.top/gtqemnxfmj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.dianchejie.cn/gtonjikenp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shzxlz.cn/gtdhxkakvu.html

[Q89] 判断表是否存在
来源：http://hz.haohaochexian.top/gtarjhwkcq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.meibo888.top/gtakvrazxe.html

[Q90] 生成序号列
来源：http://hz.jyoumei.cn/gtyywbqtef.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ivvv.top/gtktpypzvf.html

================================================================================
来源：http://hz.ppjwa.cn/gtcemdkjjc.html

R. Bash 专题
来源：http://hz.xinyue.icu/gtbnjxrnra.html

================================================================================
来源：http://hz.jqgufenzy.top/gtmfjxxurn.html

[R01] shebang 与严格模式
来源：http://hz.feifeiyinyue.top/gtghaeyvjk.html

#!/usr/bin/env bash
来源：http://hz.zhijiandao.cn/gtdyglvikc.html

set -euo pipefail
来源：http://hz.yangfankeji.com/gtyreskqcr.html

[R02] 变量赋值与使用
来源：http://hz.sweek.top/gtaodvrvnc.html

name="Tom"; echo "$name"
来源：http://hz.zhengqikj.top/gtoktoihhl.html

[R03] 只读变量
来源：http://hz.yj20258888.top/gtsypwcsre.html

readonly PI=3.14
来源：http://hz.vqdsnc.cn/gtjytqkmej.html

[R04] 位置参数
来源：http://hz.guannengcc.top/gtwpycjkco.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.meibo888.top/gtllegmmlr.html

[R05] 参数默认值
来源：http://hz.hnxiangtu.top/gtloddsord.html

name="${1:-default}"
来源：http://hz.xinyue.icu/gtadzlygtq.html

[R06] 判断命令是否存在
来源：http://hz.gzhubu.top/gtfemhlwdm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cheryme.top/gtejgthlfd.html

[R07] if 判断文件
来源：http://hz.xziqi.cn/gtxvwhdagm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenlongwang.top/gttfdjytdw.html

[R08] 数值比较
来源：http://hz.shanyushiyangkeji.top/gtuoupppwm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.wangdashe.top/gtbvzsteji.html

[R09] 字符串比较
来源：http://hz.hysaishi.cn/gtbsmktzzd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tian-w.cn/gtemrfipyq.html

[R10] 正则匹配
来源：http://hz.zdqjudy.top/gtlirdmmjy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.52xcode.cn/gtcwwmqbhz.html

[R11] case 多分支
来源：http://hz.yj20258888.top/gtvsnqmiug.html

case "$1" in
来源：http://hz.0kj1m.cn/gtfvtwkjjv.html

start) echo "启动" ;;
来源：http://hz.yangfankeji.com/gtlbhzozhz.html

stop)  echo "停止" ;;
来源：http://hz.yangfankeji.com/gtrmttofok.html

*)     echo "未知命令" ;;
来源：http://hz.gaohongyu789.top/gtshsawpnj.html

esac
来源：http://hz.sufxvd.cn/gtbtpdjtsj.html

[R12] for 遍历文件
来源：http://hz.jyoumei.cn/gtmybuuxmk.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhiwuduotai.top/gtjadchbwj.html

[R13] for 计数循环
来源：http://hz.xingfuxueyuan.xyz/gtlntpkazg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.pengpengdd.cyou/gtldsaaxom.html

[R14] C 风格 for
来源：http://hz.zhoulong.xyz/gtsvtzoxvi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.bjfxy.top/gtaxhvckmd.html

[R15] while 逐行读文件
来源：http://hz.jyoumei.cn/gtdakohgzq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yongpay.top/gtsjbjxebz.html

[R16] until 等待条件
来源：http://hz.guannengcc.top/gtmdopmfqp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shuidangran.top/gtbnktihdn.html

[R17] 数组定义与取值
来源：http://hz.cheryme.top/gtzkovsjkm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shanyushiyangtech.top/gtqxehvunx.html

[R18] 遍历数组
来源：http://hz.yanxiufei.cn/gtyxznxhkc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhijiandao.cn/gtmnbzkpye.html

[R19] 数组长度
来源：http://hz.ppjwa.cn/gtjhwfysem.html

echo "${#arr[@]}"
来源：http://hz.316326.xyz/gtpapmvyov.html

[R20] 关联数组（字典）
来源：http://hz.fzhhl.top/gtnrbjesbn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yueranfly.top/gtzlryoilb.html

[R21] 字符串长度
来源：http://hz.52xcode.cn/gtxgfaucyt.html

echo "${#s}"
来源：http://hz.zhongyouzk.top/gtfuvxnvcs.html

[R22] 截取子串
来源：http://hz.zhiwuduotai.top/gtatbrcpjt.html

echo "${s:0:5}"
来源：http://hz.jqgfzy.top/gtdatjtvuu.html

[R23] 字符串替换
来源：http://hz.yvedp.cn/gtciifgiyx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinqigfzy.top/gtygsjmhda.html

[R24] 大小写转换
来源：http://hz.cdnleiting.top/gtquujautj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.guannengcc.top/gtzmhqimwj.html

[R25] 去后缀 / 去前缀
来源：http://hz.yanxiufei.cn/gtrtzihzaj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.52xcode.cn/gtvemzvhyl.html

[R26] 命令替换
来源：http://hz.jiagoushi.top/gtumyosuot.html

now=$(date +%F); echo "$now"
来源：http://hz.cheryme.top/gtosmcplza.html

[R27] 算术展开
来源：http://hz.quarkkingdee.top/gttdlaxrzq.html

echo $((1 + 2 * 3))
来源：http://hz.tanke756.top/gtgkgyrtfb.html

[R28] 浮点运算
来源：http://hz.aibaodan.cn/gtmncezuhk.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhixingplan.top/gtdwgvrjbi.html

[R29] 定义函数
来源：http://hz.birdmap.top/gtyeulppxj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cashguo.top/gtfrfmqvms.html

[R30] 函数返回状态码
来源：http://hz.daria6918.cn/gtxsvxlflg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinqigfzy.top/gtwmtbskdz.html

[R31] 局部变量
来源：http://hz.cucudq.cn/gtqzdzypox.html

f() { local x=1; echo "$x"; }
来源：http://hz.0kj1m.cn/gtsjjzfqjx.html

[R32] 参数个数校验
来源：http://hz.ydzc1.top/gtfyeihdhk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.redwolf501.top/gtxfwppcaf.html

[R33] 捕获错误并提示行号
来源：http://hz.chenzaomai.com/gtjuzjhkez.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigufen.top/gtncjuxldx.html

[R34] 退出时清理
来源：http://hz.tian-w.cn/gtzoowjzdr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtrsxrnnea.html

[R35] 后台执行并等待
来源：http://hz.wangdashe.top/gtjkikwxub.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ydjk.org.cn/gtxutltran.html

[R36] 并发执行多个任务
来源：http://hz.yueranfly.top/gttrnhfxfl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yvedp.cn/gtjnldwetn.html

[R37] 把输出赋给变量
来源：http://hz.wangdashe.top/gtttwjczqt.html

files=$(ls -1)
来源：http://hz.sweek.top/gtqbllgfyq.html

[R38] 管道串联
来源：http://hz.aibaodan.cn/gtagipaxwx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.nanxinkj.top/gtwialmozk.html

[R39] 重定向标准输出与错误
来源：http://hz.ybcxt.top/gtbdkmkjvx.html

cmd > out.log 2>&1
来源：http://hz.gzhubu.top/gtbvauqpzx.html

[R40] 追加写日志
来源：http://hz.cashguo.top/gtytbdscdd.html

echo "log" >> out.log
来源：http://hz.ywan-chungtsiang.top/gtvrvvafgp.html

[R41] 丢弃输出
来源：http://hz.hysaishi.cn/gtopholgjb.html

cmd >/dev/null 2>&1
来源：http://hz.havefunace.top/gtsstumtar.html

[R42] 输入重定向
来源：http://hz.fengsongda.top/gtxiwaaosa.html

wc -l < a.txt
来源：http://hz.jlsjyb.cn/gtojtnhkvv.html

[R43] 按名字查找文件
来源：http://hz.svipenyu.cn/gtnbrtuuqr.html

find . -name "*.log" -type f
来源：http://hz.yuxming.cn/gtcicfobuz.html

[R44] 按修改时间查找
来源：http://hz.daxiang520.top/gtloyeijkj.html

find . -mtime -7 -type f
来源：http://hz.dianchejie.cn/gtnvhtgpgr.html

[R45] 批量删除
来源：http://hz.zhaomingkeji.xyz/gtsjcwwvzb.html

find . -name "*.tmp" -delete
来源：http://hz.xuanzx.com/gtuxycsexx.html

[R46] 递归替换文件内容
来源：http://hz.nwbrower.top/gtqlpmismb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.tanke756.top/gtnaknujbl.html

[R47] sed 单行替换
来源：http://hz.yueranfly.top/gtzurhyrvx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jyoumei.cn/gtgyckutua.html

[R48] awk 取指定列
来源：http://hz.zycfv.cn/gtharunwzl.html

awk '{print $1, $3}' a.txt
来源：http://hz.mhx1999.top/gtsjqemudd.html

[R49] awk 带条件
来源：http://hz.kuanghao11.cn/gthuvupuvb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jlsjyb.cn/gtnywzzasf.html

[R50] awk 求和
来源：http://hz.zhixingplan.top/gtkdfzlobr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hammf.cn/gtuwcuitkx.html

[R51] 排序去重取前几
来源：http://hz.xuanzx.com/gtvexqfqnk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.vqdsnc.cn/gtcdwclfqi.html

[R52] 统计行数
来源：http://hz.yueranfly.top/gtkxqyqhip.html

wc -l a.txt
来源：http://hz.yuxming.cn/gtiadentgn.html

[R53] 查看文件头与实时尾
来源：http://hz.tanke756.top/gtzytytmij.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zdqjudy.top/gtdoltcsto.html

[R54] 比较两个文件
来源：http://hz.andypj.xyz/gtpvgdnvyi.html

diff a.txt b.txt
来源：http://hz.tianlin.xyz/gtouxvldyu.html

[R55] 压缩与解压
来源：http://hz.zhixingplan.top/gtryolmeph.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xingfuxueyuan.xyz/gtitmjtxup.html

[R56] 远程拷贝
来源：http://hz.chenjidiqi.icu/gtwxjesbam.html

scp file user@host:/path/
来源：http://hz.yj20258888.top/gteuecuncn.html

[R57] 远程执行命令
来源：http://hz.yvedp.cn/gtbrrxzahr.html

ssh user@host 'uptime'
来源：http://hz.shanyushiyangtech.top/gthltrjoyk.html

[R58] 下载文件
来源：http://hz.hysaishi.cn/gtotqjioax.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhengqikj.top/gtczexofud.html

[R59] 发 POST JSON
来源：http://hz.ybcxt.top/gtitdmcncd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.snrcjt.cn/gtxoocyssl.html

[R60] 只看 HTTP 状态码
来源：http://hz.svipenyu.cn/gtzmwothjc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.smart0.xyz/gtlrjmapat.html

[R61] 磁盘占用
来源：http://hz.shangyingyoupin.top/gtzidhrilm.html

df -h;  du -sh *
来源：http://hz.dianchejie.cn/gtimdyalzq.html

[R62] 找最占空间的文件
来源：http://hz.quarkkingdee.top/gtcajgrnes.html

du -ah . | sort -rh | head -10
来源：http://hz.shanyushiyangkeji.top/gtwccijjym.html

[R63] 内存与进程
来源：http://hz.yuxming.cn/gthyqgtjfs.html

free -h;  ps aux | grep nginx
来源：http://hz.vqdsnc.cn/gtbdpxbdfd.html

[R64] 结束进程
来源：http://hz.fzhhl.top/gtqqoucdkm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.nwbrower.top/gtkkphftpb.html

[R65] 查看端口占用
来源：http://hz.hnxiangtu.top/gtvjplgkoa.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shuidangran.top/gtpxbpbcoq.html

[R66] 定时任务
来源：http://hz.xinyue.icu/gtzityagee.html

crontab -e;  crontab -l
来源：http://hz.svipenyu.cn/gtnmrctgae.html

[R67] 生成随机十六进制串
来源：http://hz.jyoumei.cn/gtcocggymk.html

openssl rand -hex 16
来源：http://hz.fengsongda.top/gtqlyaawtj.html

[R68] 计算文件校验值
来源：http://hz.shanyushiyangkeji.top/gtwrcutuuv.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhoulong.xyz/gtoelcdxrx.html

[R69] 生成随机密码
来源：http://hz.hongshengwenyu.top/gtkubuweds.html

head -c 16 /dev/urandom | base64
来源：http://hz.ybcxt.top/gtalyrwgio.html

[R70] 时间戳与互转
来源：http://hz.cqqwz.cn/gtovbnzzep.html

date +%s;  date -d @1700000000
来源：http://hz.zhoulong.xyz/gtpuezgvxn.html

[R71] 日期格式化
来源：http://hz.birdmap.top/gtwdblbyke.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cdnleiting.top/gtvvhftyvu.html

[R72] 等待端口就绪
来源：http://hz.chenzaomai.com/gtoaivlfvw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinqigufen.top/gtmhuwhuba.html

[R73] 分割大日志
来源：http://hz.gotoacloud.top/gtvtbwhkbt.html

split -l 1000 big.log part_
来源：http://hz.tianlin.xyz/gtvtuquomm.html

[R74] 批量重命名
来源：http://hz.xylfe.cn/gtuaholweg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gaohongyu789.top/gtphxsktpl.html

[R75] 导出环境变量
来源：http://hz.jinqigfzy.top/gtdpwfvcio.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sufxvd.cn/gtubfmhyvi.html

[R76] 使用临时文件
来源：http://hz.svipenyu.cn/gtfizgokrp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yongpay.top/gtgbxsflbe.html

[R77] 读取用户输入
来源：http://hz.zhongyouzk.top/gtmebpkuol.html

read -rp "请输入: " ans
来源：http://hz.jinyuanbaomall.cn/gtdnnhtkjz.html

[R78] 交互式菜单
来源：http://hz.316326.xyz/gtfzuvuira.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.aizwys.cn/gtgopcsyyt.html

[R79] 解析命令行选项
来源：http://hz.sufxvd.cn/gtxtbildpi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.feifeiyinyue.top/gtorinbsvb.html

[R80] 查看脚本执行耗时
来源：http://hz.zhengqikj.top/gtbmzxpyzy.html

time ./run.sh
来源：http://hz.redwolf501.top/gtbldbmluv.html

================================================================================
来源：http://hz.zhengqikj.top/gtgayhnhqt.html

S. C / C++ 专题
来源：http://hz.quarkkingdee.top/gtismecmep.html

================================================================================
来源：http://hz.yangfankeji.com/gttbtcjnmq.html

[S01] C：Hello World
来源：http://hz.cheryme.top/gthdlsxsuo.html

#include <stdio.h>
来源：http://hz.yuanzhike.top/gtpeyscxqy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.wangshuangyany.cn/gtywcpilan.html

[S02] C：变量与格式化输出
来源：http://hz.nanxuanxn.top/gthavkfrpv.html

int a = 10; printf("%d\n", a);
来源：http://hz.shanyushiyangtech.top/gtdqjdmxvt.html

[S03] C：读入整数
来源：http://hz.jinyuanbaomall.cn/gtmfvjasev.html

int x; scanf("%d", &x);
来源：http://hz.0kj1m.cn/gtuafabxwa.html

[S04] C：字符串复制
来源：http://hz.gogol.net.cn/gthxweknpd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yuanzhike.top/gtgfdcxixy.html

[S05] C：字符串长度
来源：http://hz.hysaishi.cn/gtqghcfiqo.html

strlen(s)
来源：http://hz.xingfuxueyuan.xyz/gtwrmycaup.html

[S06] C：字符串比较
来源：http://hz.sxryk.cn/gtkejgckuz.html

strcmp(a, b) == 0
来源：http://hz.yj20258.top/gtrvhdibcz.html

[S07] C：数组遍历求和
来源：http://hz.dashuyun.cn/gtoaoxxtfa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yj202588.top/gtiniinesr.html

[S08] C：动态内存分配与释放
来源：http://hz.hongshengwenyu.top/gtaujprnls.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ydjk.org.cn/gtxtycgujg.html

[S09] C：结构体定义与初始化
来源：http://hz.cucudq.cn/gtgvunjunj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhixingplan.top/gthskqjchq.html

[S10] C：指针与解引用
来源：http://hz.ywan-chungtsiang.top/gtrfxkqosl.html

int *p = &a;  *p = 5;
来源：http://hz.ydjk.org.cn/gtwrmpqplp.html

[S11] C：逐行读文件
来源：http://hz.sufxvd.cn/gthwrzkgzg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.9152youxi.cn/gtbthoghbc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhoulong.xyz/gtafmmdelt.html

fclose(f);
来源：http://hz.52xcode.cn/gtlegxrrqi.html

[S12] C：写文件
来源：http://hz.pengpengdd.cyou/gtjasapacm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.wangshuangyany.cn/gtomakugau.html

[S13] C：宏定义
来源：http://hz.andypj.xyz/gtrtxydtuc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ivvv.top/gtlhjngqdb.html

[S14] C：枚举
来源：http://hz.9152youxi.cn/gtlcsaftfa.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yuxming.cn/gtkdgmvtkx.html

[S15] C：类型转换
来源：http://hz.ywan-chungtsiang.top/gtoubgwhgl.html

(double) a / b
来源：http://hz.xziqi.cn/gtwpacjhls.html

[S16] C：位操作置位
来源：http://hz.hammf.cn/gteyskimwr.html

x |= (1 << 3);
来源：http://hz.cheryme.top/gtjohrjsbg.html

[S17] C：安全拼接字符串
来源：http://hz.sweek.top/gtgwugysnk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.svipenyu.cn/gtkqqioryn.html

[S18] C：命令行参数
来源：http://hz.xuanzx.com/gtrecppqxz.html

int main(int argc, char **argv)
来源：http://hz.nanxuanxn.top/gtgwzefkvc.html

[S19] C：快速排序
来源：http://hz.jlsjyb.cn/gtgvnktfbk.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jqgfzy.top/gtlehzowpx.html

[S20] C：二分查找
来源：http://hz.daria6918.cn/gthqwqmgrp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.52xcode.cn/gtipheebuv.html

[S21] C：字符类别判断
来源：http://hz.chenzaomai.com/gtpujoikfz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guannengcc.top/gtvjyxhhqw.html

[S22] C：字符串转数字
来源：http://hz.cashguo.top/gtabxudahf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.haohaochexian.top/gtavimbebl.html

[S23] C：随机数
来源：http://hz.xingfuxueyuan.xyz/gtrosmgemw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cdnleiting.top/gtzupbfwpe.html

[S24] C：获取本地时间
来源：http://hz.hfpthk.cn/gtxwdyfuaz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ydjk.org.cn/gtusytzxee.html

[S25] C：内存拷贝
来源：http://hz.svipenyu.cn/gtnkyhxhan.html

memcpy(dst, src, n);
来源：http://hz.sxryk.cn/gtulribipw.html

[S26] C：内存清零
来源：http://hz.zdqjudy.top/gtmdtphudf.html

memset(a, 0, sizeof a);
来源：http://hz.smart0.xyz/gtthalxyod.html

[S27] C：定义常量
来源：http://hz.zhengqikj.top/gttattnxjp.html

const double PI = 3.14159;
来源：http://hz.birdmap.top/gtxwpwawgd.html

[S28] C：静态变量
来源：http://hz.smart0.xyz/gtnxikekwz.html

static int counter = 0;
来源：http://hz.meibo888.top/gtrbrbgrgg.html

[S29] C：变参函数
来源：http://hz.kuanghao11.cn/gtpruovtvl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cqqwz.cn/gtjhqvhirs.html

[S30] C：头文件保护
来源：http://hz.pengpengdd.cyou/gtufidztpv.html

#ifndef X_H
来源：http://hz.jinyuanbaomall.cn/gtlmaybemv.html

#define X_H
来源：http://hz.quarkkingdee.top/gttmfuoivt.html

#endif
来源：http://hz.yj20258888.top/gtvjolqbmp.html

[S31] C++：Hello World
来源：http://hz.chenzaomai.com/gtghkaajyy.html

#include <iostream>
来源：http://hz.svipenyu.cn/gtnroitjgx.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinyuanbaomall.cn/gtdsuomskl.html

[S32] C++：字符串
来源：http://hz.yanxiufei.cn/gtlgyszbht.html

std::string s = "hi";  s += "!";
来源：http://hz.jinqigufen.top/gtimsovddb.html

[S33] C++：vector 增删
来源：http://hz.pengpengdd.cyou/gtgjbcmndq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.redwolf501.top/gtpsfoazqs.html

[S34] C++：遍历 vector
来源：http://hz.316326.xyz/gtlgekyilv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.haohaochexian.top/gtulufodvc.html


<!-- 参考信息 -->